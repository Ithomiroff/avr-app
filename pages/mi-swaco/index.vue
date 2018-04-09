<template>
  <div>
    <section class="swaco" style="background-image: url('/images/bgs/contact-bg.png')">
      <div class="title">Бентонит и буровая химия</div>

      <div class="info">Информация на продукцию американской буровой химии компании MI-SWACO Кострома</div>
      <div class="info_light">
        Посмотрите информацию: Гост (бентонит), Гост (Полимеры), приложение (Полимеры), <br>
        Прайс-лист Mi-Swaco розница Кострома
      </div>

      <div class="table-wrap">
        <table>
          <tr>
            <th>Наименование продукции</th>
            <th>Объем</th>
            <th>Паспорт качества</th>
          </tr>
          <tr>
            <td class="flex-td">
              <div class="name">Бентонит REAMAX</div>
              <span>(Высококачественный полимеризованный бентонит)</span>
              <a href="#">ПОДРОБНЕЕ</a>
            </td>
            <td>
              Мешок 25 кг
            </td>
            <td>
              Смотреть
            </td>
          </tr>
          <tr>
            <td class="flex-td">
              <div class="name">Бентонит MAX BORE HDD</div>
              <span>(Натриевый высококачественный бентонит, не требует водоподготовки)</span>
              <a href="#">ПОДРОБНЕЕ</a>
            </td>
            <td>
              Мешок 25 кг
            </td>
            <td>
              Смотреть
            </td>
          </tr>
          <tr>
            <td class="flex-td">
              <div class="name">Бентонит MAX GEL</div>
              <span>(Натриевый бентонит класса Вайоминг, основа бурового раствора)</span>
              <a href="#">ПОДРОБНЕЕ</a>
            </td>
            <td>
              Мешок 25 кг
            </td>
            <td>
              Смотреть
            </td>
          </tr>
        </table>
      </div>
    </section>

    <phone/>
    <custom-footer/>
  </div>
</template>

<script>
    import CustomFooter from "~/components/Footer";
    import Phone from "~/components/Phone";

    export default {
      components: {
        Phone,
        CustomFooter
      },
      name: "index"
    }
</script>

<style lang="scss">
  @import "../../assets/scss/mi-swaco";
</style>
