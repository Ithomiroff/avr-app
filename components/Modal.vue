<template>
  <div v-if="this.isOpenModal">
    <section class="modal-wrap">
      <div class="modal-header">
        <div class="close-btn" @click="closeModal()">
          <img src="images/icon/close-btn.svg" alt="">
        </div>
      </div>
      <div class="modal-body">
        <div class="title">Напишите нам</div>
        <div class="message">Если у вас остались вопросы, вы можете оставить сообщение, и мы с вам свяжимся.</div>
        <div class="row">
          <div class="form-wrap">
            <form action="">
              <input type="text" name="name" placeholder="Ваше полное имя*">
              <input type="text" name="phone" placeholder="Ваш телефон*">
              <input type="text" name="message" placeholder="Сообщение">

              <div>
                <div
                  class="btn"
                >
                  Отправить
                  <img src="/images/icon/mail.png" alt="">
                </div>
              </div>
            </form>
          </div>
          <div class="phone-wrap">
            <div class="text">Или позвоните нам:</div>
            <div class="phone">
              <img src="images/icon/phone-white.svg" alt="">
              +7 (4942) 300-376
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
    export default {
      name: "modal",
      props: ['isOpenModal'],
      data() {
        return {
        }
      },
      methods: {
        closeModal() {
          this.isOpenModal = !this.isOpenModal;
        }
      }
    }
</script>

<style lang="scss">
  @import "../assets/scss/mixin";

  .modal-wrap {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100vh;
    z-index: 1000;

    display: flex;
    flex-direction: column;
    justify-content: center;

    background-image: url('/images/bgs/write-us-bg.png');
    background-size: cover;
    background-position: center;
    color: #ffffff;
    @media (max-width: 769px) {

    }
    .close-btn {
      cursor: pointer;
      img {
        width: 100%;
        max-width: 100px;
        @media (max-width: 769px) {
          max-width: 40px;
        }
      }
    }

    .modal-header {
      position: relative;
      display: flex;
      justify-content: flex-end;
    }

    .modal-body {
      .title {
        @include title(#fff);
      }
      .row {
          display: flex;
          flex-direction: row;
          align-items: center;
          @media (max-width: 769px) {
            flex-direction: column;
            align-items: normal;
          }
      }
      .phone-wrap {
          flex-basis: 50%;
          text-align: center;
      }
      .form-wrap {
          flex-basis: 50%;
        form {
          display: flex;
          flex-direction: column;
          input {
            background-color: transparent;
            border: 0;
            border-bottom: 1px solid #fff;
            padding: 10px;
            color: #ffffff;
            margin-bottom: 20px;
            width: 70%;
            @media (max-width: 769px) {
              width: 100%;
            }
          }
          @media (max-width: 769px) {
            margin-bottom: 30px;
          }
        }
      }
      .message {
          margin: 40px 0;
      }

      .close-btn {
          text-align: right;
          cursor: pointer;
      }
    }


    ::-webkit-input-placeholder { /* Chrome/Opera/Safari */
        text-transform: uppercase;
        font-weight: 600;
        color: #ffffff;
    }
    ::-moz-placeholder { /* Firefox 19+ */
        text-transform: uppercase;
        font-weight: 600;
        color: #ffffff;
    }
    :-ms-input-placeholder { /* IE 10+ */
        text-transform: uppercase;
        font-weight: 600;
        color: #ffffff;
    }
    :-moz-placeholder { /* Firefox 18- */
        text-transform: uppercase;
        font-weight: 600;
        color: #ffffff;
    }
  }
  /*.modal-wrap {*/

    /*position: fixed;*/
    /*top: 0;*/
    /*left: 0;*/
    /*z-index: 1000;*/
    /*width: 100%;*/
    /*height: 100vh;*/
    /*background-image: url('/images/bgs/write-us-bg.png');*/
    /*background-size: cover;*/
    /*background-position: center;*/
    /*color: #ffffff;*/
  /*}*/
  /*.modal-header {*/
    /*position: relative;*/
    /*display: flex;*/
    /*justify-content: flex-end;*/
  /*}*/
  /*.row {*/
    /*display: flex;*/
    /*flex-direction: row;*/
    /*align-items: center;*/
  /*}*/
  /*.phone-wrap {*/
    /*flex-basis: 50%;*/
    /*text-align: center;*/
  /*}*/
  /*.form-wrap {*/
    /*flex-basis: 50%;*/
  /*}*/
  /*form {*/
  /*}*/
  /*.message {*/
    /*margin: 40px 0;*/
  /*}*/

  /*.close-btn {*/
    /*text-align: right;*/
    /*cursor: pointer;*/
  /*}*/

  /*::-webkit-input-placeholder { !* Chrome/Opera/Safari *!*/
    /*text-transform: uppercase;*/
    /*font-weight: 600;*/
    /*color: #ffffff;*/
  /*}*/
  /*::-moz-placeholder { !* Firefox 19+ *!*/
    /*text-transform: uppercase;*/
    /*font-weight: 600;*/
    /*color: #ffffff;*/
  /*}*/
  /*:-ms-input-placeholder { !* IE 10+ *!*/
    /*text-transform: uppercase;*/
    /*font-weight: 600;*/
    /*color: #ffffff;*/
  /*}*/
  /*:-moz-placeholder { !* Firefox 18- *!*/
    /*text-transform: uppercase;*/
    /*font-weight: 600;*/
    /*color: #ffffff;*/
  /*}*/

  /*@media (max-width: 690px) {*/
    /*.row {*/
      /*flex-direction: column;*/
    /*}*/

    /*.phone-wrap {*/
      /*margin-top: 50px;*/
    /*}*/
  /*}*/
  /*@media (max-width: 500px) {*/
    /*.close-btn img {*/
      /*width: 50%;*/
    /*}*/
  /*}*/
  /*@media (max-width: 390px) {*/
    /*.modal-wrap {*/
      /*justify-content: unset;*/
      /*overflow-y: auto;*/
    /*}*/
    /*.modal-header {*/
      /*margin-bottom: 45px;*/
    /*}*/
  /*}*/
</style>
