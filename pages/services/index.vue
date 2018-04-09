<template>
  <div>
    <section class="service" style="background-image: url('/images/bgs/service-bg.jpg')">
      <div class="overlay"></div>

      <div class="service-wrap">
        <div class="title">Услуги</div>
        <div class="text">Прокладка труб методом Горизонтально направленного бурения (ГНБ) </div>

        <div class="service-content">
          <div class="table-wrap">
            <table>
              <tr>
                <th>Диаметр трубы, мм</th>
                <th>Стоимость, руб</th>
              </tr>
              <tr>
                <td>Ø 63</td>
                <td>2 000</td>
              </tr>
              <tr>
                <td>Ø 110</td>
                <td>2 500</td>
              </tr>
              <tr>
                <td>Ø 160</td>
                <td>3 000</td>
              </tr>
              <tr>
                <td>Ø 225</td>
                <td>4 000</td>
              </tr>
              <tr>
                <td>Ø 315</td>
                <td>5 000</td>
              </tr>
              <tr>
                <td>Ø 400</td>
                <td>6 300</td>
              </tr>
              <tr>
                <td>Ø 500</td>
                <td>11 300</td>
              </tr>
              <tr>
                <td>Ø 630</td>
                <td>13 000</td>
              </tr>
              <tr>
                <td>Ø 710</td>
                <td>от 18 000</td>
              </tr>
            </table>
          </div>
          <div class="text-wrap">
            По всем интересующим вопросам звоните по телефонам: <br>
            <span>+7 (4942) 300-376</span>
          </div>
        </div>
      </div>
    </section>

    <phone/>
    <custom-footer/>
  </div>
</template>

<script>
    import CustomFooter from "~/components/Footer.vue";
    import Phone from "~/components/Phone";

    export default {
      components: {
        Phone,
        CustomFooter
      },
      name: "index",
    }
</script>

<style lang="scss">
  @import "../../assets/scss/services";
</style>
