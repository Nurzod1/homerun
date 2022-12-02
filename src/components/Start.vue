<template>
  <div class="start">
    <div class="container">
      <div class="start-wrapper">
        <div class="start-image">
          <img src="../assets/img/dog.png" alt="" />
        </div>
        <div class="start-title">Start your free Homerun trial today</div>
        <div class="start-btn">
          <Button title="Start free trial" />
        </div>
        <div class="start-bonusess">
          <div class="start-bonusess__text">
            <img src="../assets/img/Frame3.svg" alt="" />
            <p>Totally free for 15 days</p>
          </div>
          <div class="start-bonusess__text">
            <img src="../assets/img/Frame3.svg" alt="" />
            <p>No credit card needed</p>
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
  name: "Start",
};
</script>

<style lang="scss" scoped>
.start {
  color: white;
  &-wrapper {
    display: flex;
    flex-direction: column;
    gap: 20px;
    padding: 70px 10px;
    align-items: center;
    background-color: #3ca9ff;
    border-radius: 20px;
    text-align: center;
    @include breakpoint(sm) {
      padding: 40px 10px;
    }
  }
  &image {
    img {
      width: 100%;
      height: 100%;
    }
  }
  &-title {
    font-size: 57px;
    line-height: 63px;
    max-width: 556px;
    @include breakpoint(md) {
      font-size: 46px;
      line-height: 57px;
    }
    @include breakpoint(sm) {
      font-size: 36px;
      line-height: 47px;
    }
    @media screen and (max-width: 415px) {
      font-size: 28px;
      line-height: 38px;
    }
  }
  &-bonusess {
    display: flex;
    gap: 20px;
    @include breakpoint(sm){
      gap: 10px;
    }
    &__text {
      display: flex;
      align-items: center;
      gap: 5px;
      @include breakpoint(xs){
        gap: 0px;
      }
      p {
        @include breakpoint(md) {
          font-size: 14px;
          line-height: 18px;
        }
        @media screen and (max-width: 415px) {
          font-size: 10px;
          line-height: 14px;
        }
      }
    }
  }
  button {
    cursor: pointer;
    transition: 0.3s;
    font-size: 16px;
    font-weight: 500;

    &:hover {
      border-color: #000;
    }
  }
}
</style>