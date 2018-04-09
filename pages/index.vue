<template>
    <div>
      <section class="top" style="background-image: url('/images/bgs/video.png')">
        <div class="top-text">
          <div class="top-text__title">ПРОКЛАДКА И РЕМОНТ ТРУБОПРОВОДОВ</div>
          <div class="top-text__desc">В КОСТРОМСКОЙ, ИВАНОВСКОЙ И ЯРОСЛАВСКИХ ОБЛАСТЯХ</div>
        </div>
      </section>

      <section class="projects">
        <div class="title">Проекты</div>
        <div class="projects__desc g-text">
          <div class="digit">50</div>
          <div class="text">успешных <br> проектов</div>
        </div>
        <div class="projects-wrap">
          <div class="item">
            <div class="item__head">
              Сотрудники компании "Авр центр" за 2017 год  уже побывали в
            </div>
            <div class="item__body">
              <div class="g-text">
                <div class="digit">43-x</div>
              </div>
            </div>
            <div class="item__footer">
              Городах
            </div>
          </div>
          <div class="item" style="background-image: url('/images/item.png')">
          </div>
          <div class="item">
            <div class="item__head">
              Выполняя поручения клиентов,  компания  "Авр центр"  в 2017 году покрыла расстояние в
            </div>
            <div class="item__body">
              <div class="g-text">
                <div class="digit">4</div>
                <div class="text">раза больше</div>
              </div>
            </div>
            <div class="item__footer">
              чем другие компании по области
            </div>
          </div>
        </div>

        <div class="projects-link">
          <router-link :to="{ name: 'projects' }">
            <span style="text-transform: uppercase;">Все проекты</span>
          </router-link>
        </div>
      </section>

      <slider-partners/>

      <custom-footer/>

    </div>
</template>

<script>
    import CustomFooter from "~/components/Footer.vue";
    import SliderPartners from "~/components/SliderPartners.vue";

    export default {
      components: {
        SliderPartners,
        CustomFooter,
      },
      mounted() {

      }
    }
</script>

<style lang="scss">
  @import "../assets/scss/index";
</style>
