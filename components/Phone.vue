<template>
  <section class="question">
    <div class="have-question">
      <div class="text">Есть вопросы?/Нужна консультация?</div>
      <div class="button-wrap">
        <div class="nav__btn">
          <div
            class="btn"
            @click = "openModal()"
          >
            Напишите нам
            <img src="/images/icon/mail.png" alt="">
          </div>
        </div>
      </div>
    </div>

    <div class="phone">
      <img src="/images/phone-service.png" alt="">
    </div>

  </section>
</template>

<script>
    export default {
        name: "phone",
    }
</script>

<style lang="scss">
  .question {
    display: flex;
    align-items: center;
    justify-content: space-between;
    @media (max-width: 600px) {
      flex-direction: column;
      justify-content: center;
      text-align: center;
      .text {
        margin: 0;
      }
    }

    .have-question {
      .text {
        margin-bottom: 30px;
        font-weight: 600;
        font-size: 20px;
      }
    }
    .phone {
      img {
        animation: top-bottom 3s infinite ease-in-out;
        width: 100%;
      }
    }
  }
  .nav__btn {
    margin-top: 40px !important;
  }

  @keyframes top-bottom {
    0%   {transform: translateY(0);}
    50% {transform: translateY(-6%);}
    100% {transform: translateY(0);}
  }
</style>
