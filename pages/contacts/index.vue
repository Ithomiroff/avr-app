<template>
  <div>
    <section class="contact" style="background-image: url('images/bgs/contact-bg.png')">
      <div class="title">Контакты</div>

      <div class="contact-info">
        <div class="contact-info__header">
          <div class="heading">Есть вопросы?</div>
        </div>
        <div class="contact-info__body">
          <div class="row">
            <div class="phone_big">
              <div class="text-big">+7 (4942) 300-376</div>
              <span>Круглосуточный</span>
            </div>
            <div class="phone_small">
              <div class="text-small">+7 (4942) 472-474</div>
              <span>Номер факса</span>
            </div>
          </div>
          <div class="row">
            <div class="mail_big">
              <div class="text-big">avr@avr-centr.ru</div>
              <span>Почта компании</span>
            </div>
            <div class="mail_small">
              <div class="text-small">avr.centr@yandex.ru</div>
              <span>Почта бухгалтерии</span>
            </div>
          </div>
        </div>
      </div>

      <div class="contact-footer">
        <div class="address">
          <div class="address-header">
            Адрес офиса:
          </div>
          <div class="address-content">
            <div class="address-content__marker">
              <img src="/images/icon/marker-o.svg" alt="">
            </div>
            <div class="address-content__text">
              ул. Нижняя Дебря, 58, номер 309, <br>
              Кострома, Костромская обл., 156005
            </div>
          </div>
        </div>

        <div class="address">
          <div class="address-header">
            Адрес склада:
          </div>
          <div class="address-content">
            <div class="address-content__marker">
              <img src="/images/icon/marker-c.svg" alt="">
            </div>
            <div class="address-content__text">
              Кинешемское ш., 4А, Кострома, <br>
              Костромская обл., 156019
            </div>
          </div>
        </div>
      </div>
    </section>

    <div id="map">
      <gmap-map
        :center="{lat:57.755495, lng:40.962386}"
        :zoom="12"
        style="width: 100%; height: 100%"
      >
        <gmap-marker
          :key="index"
          v-for="(m, index) in markers"
          :position="m.position"
          :clickable="true"
          :draggable="true"
          :icon="m.icon"
        ></gmap-marker>
      </gmap-map>
    </div>

    <custom-footer/>
  </div>
</template>

<script>
    import CustomFooter from "~/components/Footer";

    export default {
      components: {
        CustomFooter,
      },
      name: "index",
      data() {
        return {
          markers: [{
            position: {lat: 57.758008, lng: 40.941261},
            icon: '/images/icon/marker-c.svg'
          },{
            position: {lat: 57.754171, lng: 40.983384},
            icon: '/images/icon/marker-o.svg'
          }]
        }
      },
      mounted() {

      },
    }
</script>

<style lang="scss">
  @import "../../assets/scss/contacts";
</style>
