<template>
  <div class="hire">
    <div class="container">
      <div class="hire-wrapper">
        <div class="hire-about">
          <div class="hire-about__subtitle">Hire</div>
          <div class="hire-about__title">
            An all-in-one tool for your entire team.
          </div>
          <div class="hire-about__text">
            No more ping-ponging between emails, spreadsheets, and other apps.
            Bring everything together in one place.
          </div>
          <Button title="Learn more" />
        </div>
        <div class="hire-media">
          <div class="hire-media__img">
            <img src="../assets/img/Frame.png" alt="" />
          </div>
          <div class="hire-media__text">
            All your jobs, candidates, messages and notes in one place.
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
  name: "Hire",
};
</script>

<style lang="scss" scoped>
.hire {
  &-wrapper {
    display: flex;
    justify-content: center;
    gap: 10px;
    align-items: center;
    @media screen and (max-width: 486px){
      flex-direction: column;
    }
  }
  &-about {
    display: flex;
    flex-direction: column;
    gap: 20px;
    @include breakpoint(lg) {
      gap: 10px;
    }
    &__subtitle {
      font-size: 30px;
      line-height: 36px;
      font-weight: 700;
      color: #0c9f64;
      @include breakpoint(lg) {
        font-size: 24px;
        line-height: 25px;
      }
      @include breakpoint(sm) {
        font-size: 18px;
        line-height: 22px;
      }
    }
    &__title {
      font-size: 56px;
      line-height: 63px;
      font-weight: 700;
      letter-spacing: 1.5px;
      max-width: 369px;
      @include breakpoint(lg) {
        font-size: 42px;
        line-height: 48px;
        letter-spacing: 1px;
      }
      @include breakpoint(sm) {
        font-size: 28px;
        line-height: 30px;
        letter-spacing: 0px;
      }
    }
    &__text {
      font-size: 20px;
      line-height: 30px;
      max-width: 392px;
      @include breakpoint(lg) {
        font-size: 14px;
        line-height: 20px;
      }
    }
  }
  &-media {
    display: flex;
    flex-direction: column;
    gap: 10px;
    text-align: center;
    &__img {
      img {
        width: 100%;
        height: 100%;
      }
    }
    &__text {
      font-size: 16px;
      line-height: 20px;
      color: #0e101666;
    }
  }

  button {
    cursor: pointer;
    transition: 0.3s;

    &:hover {
      border-color: #000;
    }
  }
}
</style>