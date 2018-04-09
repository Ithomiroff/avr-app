<template>
  <div>
    <button
      class="custom-hum hamburger hamburger--collapse"
      type="button"
      :class="{'is-active': this.isMenuOpen}"
      @click="toogleMenu()"
    >
              <span class="hamburger-box">
                <span class="hamburger-inner"></span>
              </span>
    </button>
    <div
      class="nav"
      :class="{'nav-media': this.isMenuOpen}"
    >
      <div class="nav__logo"><img src="images/logo.png" alt=""></div>
      <div class="nav__ul">
        <ul>
          <li v-for="(link, index) of this.links" :key="index">
            <router-link :to="{ name: link.route }" exact>
              <span style="text-transform: uppercase;">{{link.name}}</span>
            </router-link>
          </li>
        </ul>
      </div>
      <div class="nav__btn">
        <div
          @click="openModal()"
          class="btn"
        >
          Напишите нам
          <img src="/images/icon/mail.png" alt="">
        </div>
      </div>
      <div class="nav__phone">
        <img src="images/icon/phone.png" alt="">
        +7 (4942) 300-376
      </div>
      <div class="nav__desc">получи бесплатную консультацию</div>
    </div>

    <modal
    :isOpenModal="this.isOpenModal"
    ></modal>

  </div>
</template>

<script>
    import Modal from "~/components/Modal";

    export default {
      components: {Modal},
      name: "navbar",
        data() {
            return {
                'isOpenModal': false,
                'isMenuOpen': false,
                'links': [
                {
                  id:1,
                  name:'главная',
                  route: 'index'
                },
                {
                  id:2,
                  name:'проекты',
                  route: 'projects'
                },
                {
                  id:3,
                  name:'о компании',
                  route: 'about'
                },
                {
                  id:4,
                  name:'услуги',
                  route: 'services'
                },
                {
                  id:5,
                  name:'mi - swaco',
                  route: 'mi-swaco'
                },
                {
                  id:6,
                  name:'Контакты',
                  route: 'contacts'
                }
          ]
        }
      },
      methods: {
          toogleMenu() {
            this.isMenuOpen = !this.isMenuOpen;
          },
          openModal() {
            this.isOpenModal = false;
            this.isOpenModal = true;
          }
      }
    }
</script>

<style lang="scss">
  @import "../assets/scss/navbar";
</style>
