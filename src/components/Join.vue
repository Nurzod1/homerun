<template>
  <div class="join">
    <div class="container">
      <div class="join-wrapper">
        <div class="join-intro">
          <div class="join-intro__logo">
            <img src="../assets/img/logo1.png" alt="" />
          </div>
          <div class="join-intro__title">Join the club.</div>
          <div class="join-intro__text">
            Homerun customers share a passion for culture, design and
            innovation. We all agree hiring can be more meaningful and personal.
          </div>
          <Button title="About our customers" />
        </div>
        <div class="join-slider">
          <div class="join-slider__img">
            <img src="../assets/img/person.png" alt="" />
          </div>
          <div class="join-about">
            <div class="join-about__logo">
              <img src="../assets/img/logo2.png" alt="" />
            </div>
            <div class="join-about__text">
              “You don't need to be a pro in HR or even in Homerun to be able to
              use it. It's so easy that anyone in the team can figure it out.”
            </div>
            <div class="join-about__autor">Isabel Machielse</div>
            <div class="join-about__category">People & Culture Coordinator</div>
            <Button title="Read customer story" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Button from "./Button.vue";
export default {
  components: { Button },
  name: "Join",
};
</script>

<style lang="scss" scoped>
.join {
  color: #fff;
  &-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #202e78;
    border-radius: 20px;
    padding: 40px;
  }
  &-intro {
    display: flex;
    flex-direction: column;
    gap: 30px;
    padding: 20px 0;
    align-items: center;
    @include breakpoint(md) {
      gap: 20px;
    }
    &__title {
      font-size: 56px;
      line-height: 63px;
      letter-spacing: 1.5px;
      font-weight: 700;
      @include breakpoint(md) {
        font-size: 36px;
        line-height: 42px;
        letter-spacing: 1px;
      }
      @include breakpoint(xs) {
        font-size: 24px;
        line-height: 28px;
        letter-spacing: 0px;
      }
    }
    &__text {
      font-size: 22px;
      line-height: 30px;
      max-width: 719px;
      text-align: center;
      @include breakpoint(md) {
        font-size: 18px;
        line-height: 24px;
      }
      @include breakpoint(xs) {
        font-size: 14px;
        line-height: 18px;
      }
    }
  }
  &-slider {
    display: flex;
    background-color: #000639;
    border-radius: 20px;
    @include breakpoint(sm){
      flex-direction: column;
    }
    &__img {
      img {
        width: 100%;
        height: 100%;
        @include breakpoint(sm){
          border-radius: 8px;
        }
      }
    }
  }
  &-about {
    padding: 40px;
    display: flex;
    flex-direction: column;
    gap: 40px;
    @include breakpoint(lg) {
      gap: 20px;
    }
    @include breakpoint(md) {
      gap: 10px;
    }
    &__text {
      font-size: 30px;
      line-height: 36px;
      max-width: 470px;
      @include breakpoint(lg) {
        font-size: 22px;
        line-height: 28px;
      }
      @include breakpoint(md) {
        font-size: 18px;
        line-height: 22px;
      }
      @media screen and (max-width: 520px){
        font-size: 16px;
        line-height: 20px;
      }
    }
    &__autor {
      font-size: 22px;
      line-height: 30px;
      @include breakpoint(lg) {
        font-size: 16px;
        line-height: 22px;
      }
      @include breakpoint(md) {
        font-size: 14px;
        line-height: 20px;
      }
    }
    &__category {
      font-size: 22px;
      line-height: 30px;
      @include breakpoint(lg) {
        font-size: 16px;
        line-height: 22px;
      }
      @include breakpoint(md) {
        font-size: 14px;
        line-height: 20px;
      }
    }
  }

  button {
    cursor: pointer;
    transition: 0.3s;
    border-color: #fff;
    &:hover {
      background-color: #fff;
      color: #202e78;
      border-color: #202e78;
    }

    &:nth-child(2){
     &:hover {
      background-color: #fff;
      color: #000639;
      border-color: #000639;
    } 
    }
  }
}
</style>