<script setup>
import HeaderComponent from "./components/HeaderComponent.vue";
</script>

<template>
  <HeaderComponent />

  <main>
    <div class="hero">
      <div class="hero__background"></div>
      <div class="hero__container">
        <span class="hero__title">
          <div>
            <p>Hey there,</p>
            <p>I'm <span class="hero__title__name"> Yasmim </span></p>
          </div>
          <img
            class="hero__title__mobile"
            src="./assets/profile.png"
            alt="profile picture with programming languages"
          />
        </span>
        <span class="hero__profile">
          <img
            src="./assets/profile.png"
            alt="profile picture with programming languages"
          />
        </span>
      </div>
    </div>
    <div class="services">
      <span class="services__title">
        <div>
          <p>Hey there,</p>
          <p>I'm <span class="services__title__name"> Yasmim </span></p>
        </div>
      </span>
      <span class="services__profile"> </span>
    </div>
  </main>
</template>

<style lang="scss" scoped>
.hero {
  &__icons {
    display: flex;
    position: relative;
  }
  &__profile {
    img {
      height: auto;
      width: 400px;
      right: 0;
      position: absolute;
      @media (max-width: 767px) {
        display: none;
      }
      @media (min-width: 901px) {
        right: 5%;
      }
      @media (min-width: 700px) and (max-width: 900px) {
        right: 2%;
        width: 350px;
      }
    }
  }
  &__container {
    width: 100vw;
    display: flex;
    @media (max-width: 625px) {
      width: 100%;
    }
  }
  &__title {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    z-index: 1;
    width: 700px;
    font-size: clamp(2.8125rem, -1.4844rem + 8.5938vw, 6.25rem);
    height: 450px;
    padding-left: 50px;
    @media (max-width: 767px) {
      display: flex;
      padding: 0;
      align-items: center;
      flex-direction: row;
    }
    &__mobile {
      width: 300px;
      padding-left: 20px;
      @media (min-width: 767px) {
        display: none;
      }
    }
    p {
      margin: 0;
      padding: 20px;
    }
    &__name {
      color: #a175e9;
    }
  }
  &__background {
    background-color: #262626;
    position: absolute;
    border-top-right-radius: 300px;
    border-bottom-right-radius: 300px;
    width: 50%;
    height: 450px;
    z-index: 0;
    @media (min-width: 320px) and (max-width: 767px) {
      width: 100%;
      border-top-right-radius: 0;
      border-bottom-right-radius: 0;
    }
    // @media (min-width: 320px) {
    //   padding: 0;
    // }
  }
}
.services {
  height: 700px;
}
</style>
