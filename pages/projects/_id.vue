<template>
  <div class="detail-wrap">
    <div class="gallery">
      <img src="/images/detail-image.png" alt="">
      <img src="/images/detail-image.png" alt="">
      <img src="/images/detail-image.png" alt="">
    </div>
    <div class="description">
      <div class="head">
        <div class="close-btn"
             v-on:click = "closeProject()"
        >
          <img src="/images/icon/close-btn.svg" alt="">
        </div>
      </div>
      <div class="body">
        <div class="project__title">
          Прокладка газопровода,
          деревня Расторопово
        </div>
        <div class="date">
          1 АПРЕЛЯ 2015
        </div>
        <div class="text">
          Одним из объектов, выполненных методом ГНБ, была прокладка газопровода
          диметром 110мм в районе деревни Расторопово Ярославской области общей
          протяженностью 1300м. Прокладка проходила в условиях сильно обводненных и заболоченных грунтов, под дорогами и малыми реками с использованием
          самоходной установки GRUNDODRILL 7X.
        </div>
        <div class="next-project-btn">
          <div
            @click="this.nextProject()"
            class="btn__next"
          >
            Следующий проект
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: "project_id",
        mounted() {
          let content =
            document.querySelector('.content');
          content.style = 'padding-left: 0';

          let nav =
            document.querySelector('.nav');
          nav.style = 'display: none';
        },
        methods: {
          closeProject () {
            this.$router.go(-1);
          },
          nextProject () {

          }
        }
    }
</script>

<style lang="scss">
  @import "../../assets/scss/detail-project";
</style>
