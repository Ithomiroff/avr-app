<template>
  <div>
    <section class="about-wrap">
      <div class="title">о компании</div>
      <div class="about-header">
        <div class="about-header__info">
          <div class="flex-cont">
            <div class="about-desc">
              <div class="first-text">
                <div class="letter">
                  <img src="/images/icon/letter.svg" alt="">
                </div>
                <div class="text">
                  сновным видом деятельности группы компаний «АВР-Центр»  является прокладка и ремонт трубопроводов в Костромской, Ивановской и
                  Ярославской областях.
                </div>
              </div>
              <div class="second-text">
                <p>
                  Специализация компании на бестраншейной прокладке полиэтиленовых и стальных трубопроводов для нужд водоканализационного хозяйства, футляры для электроэнергетических кабельных линий, футляры для телекоммуникационных линий и газопроводы.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="about-body">
        <div class="row">
          <div class="row-text" style="order: 1">
            <div class="row-text__img">
              <img src="/images/icon/Vector1.svg" alt="">
            </div>
            <div class="row-text__title">Лучшие специалисты</div>
            <div class="row-text__text">
              Главный актив, постоянно проводится обучение персонала новым методам работы и применение передовых технологий бурения.
            </div>
          </div>
          <div class="row-word" style="order: 2">
            качество
          </div>
        </div>

        <div class="row">
          <div class="row-text" style="order: 2">
            <div class="row-text__img">
              <img src="/images/icon/Vector2.svg" alt="">
            </div>
            <div class="row-text__title">Рост компании</div>
            <div class="row-text__text">
              Результат работы компании — Рекомендации наших Заказчиков. Свыше 80% заказов в год приходится на наших постоянных партнеров, что при постоянно растущем портфеле заказов.
            </div>
          </div>
          <div class="row-word" style="order: 1">
            надежность
          </div>
        </div>

        <div class="row">
          <div class="row-text" style="order: 1">
            <div class="row-text__img">
              <img src="/images/icon/Vector3.svg" alt="">
            </div>
            <div class="row-text__title">Участие в проектах</div>
            <div class="row-text__text">
              Компания приняла участие во всех значимых проектах в городе Костроме, Мантурово, Волгореченске, Галиче - ремонт автопешеходного моста, строительство жилых микрорайонов, реконструкция сетей ГРЭС и МРСК, прокладка сетей для новых и существующих современных промышленных и коммунальных предприятий.
            </div>
          </div>
          <div class="row-word" style="order: 2">
            профессионализм
          </div>
        </div>

        <div class="bottom">
          <div class="bottom__hidden-text">
            «АВР-Центр»
          </div>
          <div class="bottom__top-text">
            <strong>МЫ РАСТЕМ ВМЕСТЕ</strong> <br>
            С НАШИМИ ЗАКАЗЧИКАМИ
          </div>
        </div>
      </div>
    </section>

    <section class="how-work">
      <div class="how-work__head">
        <div class="title">как мы работаем</div>
        <div class="text">
          Вместе с заказчиком отвечаем на <strong>следующие вопросы</strong>
        </div>
      </div>
      <div class="how-work__body">
        <div class="row">
          <div class="work-item">
            <div class="work-item__title">Наличие проекта и разрешительной документации</div>
            <div class="work-item__text">
              Оказываем содействие Заказчику в получении всех необходимых документов.
            </div>
            <div class="work-item__digit">1</div>
          </div>
          <div class="work-item">
            <div class="work-item__title">Общие вопросы</div>
            <div class="work-item__text">
              Вид прокладываемых коммуникаций, диаметр трубопроводов, протяженность, наличие инженерных сооружений на сети (колодцы, КСН, очистные сооружения). Мы придерживаемся комплексного подхода «под ключ» в строительстве объекта со сдачей контролирующим органам и сетевым организациям.
            </div>
            <div class="work-item__digit">2</div>
          </div>
        </div>
        <div class="row">
          <div class="work-item">
            <div class="work-item__title">Информация об объекте</div>
            <div class="work-item__text">
              Определение на объекте способа и сроков выполнения работ, комплектации необходимыми материалами. Мы имеем наработанные связи с Поставщиками качественных материалов, предоставляющим гарантии на поставленные материалы.
            </div>
            <div class="work-item__digit">3</div>
          </div>
          <div class="work-item">
            <div class="work-item__title">Стоимость проекта</div>
            <div class="work-item__text">
              Обсуждение с Заказчиком стоимости проекта с учетом привлечения спецтехники и субподрядчиков, индивидуальных особенностей проекта.
              Мы предлагаем комфортные финансовые условия
              по оплате производимых работ
            </div>
            <div class="work-item__digit">4</div>
          </div>
        </div>

        <div class="row done-block" style="justify-content: center">
          <div class="icon">
            <img src="/images/icon/group.svg" alt="">
          </div>
          <div class="desc">
            В результате тщательной подготовки Заказчик получает <br>
            <strong>качественный готовый объект</strong> в оптимальные сроки по разумной цене.
          </div>
        </div>
      </div>
    </section>

    <section class="team">
      <div class="title">Команда</div>
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
        CustomFooter
      },
      name: "index"
    }
</script>

<style lang="scss">
  @import "../../assets/scss/about";
</style>
