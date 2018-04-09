<template>
  <div>
    <div class="projects-page">
      <div class="item-wrap"
           v-for="project in projects"
           v-bind:key="project.id"
           v-on:mouseover = "mouseOver(project)"
           v-on:mouseleave = "mouseLeave(project)"
           v-on:click = "chooseProject(project)"
           v-bind:class="{ overlay: project.active}"
      >
        <div class="item">
          <img :src="project.style" alt="">
        </div>
        <div class="item__title" v-if="project.active">
          {{project.name}}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: "index",
        data() {
          return {
            projects : [
              {
                id: 1,
                name: 'abr',
                style: '/images/item.png',
                active: false
              },
              {
                id: 2,
                name: 'abr',
                style: '/images/item.png',
                active: false
              },
              {
                id: 3,
                name: 'abr',
                style: '/images/item.png',
                active: false
              },
              {
                id: 4,
                name: 'abr',
                style: '/images/item.png',
                active: false
              }
              ,
              {
                id: 5,
                name: 'abr',
                style: '/images/item.png',
                active: false
              }
              ,
              {
                id: 6,
                name: 'abr',
                style: '/images/item.png',
                active: false
              }
              ,
              {
                id: 7,
                name: 'abr',
                style: '/images/item.png',
                active: false
              }
              ,
              {
                id: 8,
                name: 'abr',
                style: '/images/item.png',
                active: false
              }
              ,
              {
                id: 9,
                name: 'abr',
                style: '/images/item.png',
                active: false
              }
              ,
              {
                id: 10,
                name: 'abr',
                style: '/images/item.png',
                active: false
              }
            ]
          }
        },
        mounted() {
          let content =
            document.querySelector('.content');
          content.style = 'padding-left: 25vw';

          let nav =
            document.querySelector('.nav');
          nav.style = 'display: flex';
        },
        methods: {
          mouseOver: function (project) {
            project.active = true;
          },
          mouseLeave: function (project) {
            project.active = false;
          },
          chooseProject: function (project) {
            this.$router.push({name:'projects-id', params: { id: project.id }});
          },
        }
    }
</script>

<style lang="scss">
  @import "../../assets/scss/projects";
</style>
