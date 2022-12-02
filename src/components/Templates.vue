<template>
  <div class="templates">
    <div class="container">
      <div class="templates-wrapper">
        <div class="templates-about">
          <div class="templates-about__new">
            <p>new</p>
          </div>
          <div class="templates-about__title">
            Kickstart hiring <br />
            with Homerun templates.
          </div>
          <div class="templates-about__text">
            Ready to use job templates to help you with the hardest parts of
            creating a job post.
          </div>
          <Button title="Explore all templates" />
        </div>
        <div class="templates-img">
          <img src="../assets/img/image.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Button from "./Button.vue";
export default {
  components: { Button },
};
</script>

<style lang="scss" scoped>
.templates {
  &-wrapper {
    padding-top: 70px;
    background-color: #181818;
    border-radius: 20px;
    color: #fff;
    @include breakpoint(sm){
     padding-top: 30px;
    }
  }
  &-about {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 0px 20px;
    gap: 30px;
    @include breakpoint(sm){
      gap: 10px;
    } 
    &__new {
      display: flex;
      justify-content: center;
      text-align: center;
      p {
        width: 62px;
        height: 32px;
        background-color: #f64775;
        border-radius: 20px;
        padding: 5px;
        @include breakpoint(sm) {
          width: 42px;
          height: 26px;
          font-size: 14px;
        }
      }
    }
    &__title {
      font-size: 58px;
      line-height: 63px;
      letter-spacing: 1.5px;
      font-weight: 700;
      max-width: 708px;
      text-align: center;
      @include breakpoint(md) {
        font-size: 46px;
        line-height: 56px;
        letter-spacing: 1px;
      }
      @include breakpoint(sm) {
        font-size: 36px;
        line-height: 46px;
        letter-spacing: 0px;
      }
      @include breakpoint(xs) {
        font-size: 26px;
        line-height: 36px;
        letter-spacing: 0px;
      }
      @media screen and (max-width: 385px) {
        font-size: 22px;
        line-height: 28px;
      }
    }
    &__text {
      font-size: 22px;
      line-height: 30px;
      max-width: 441px;
      text-align: center;
      @include breakpoint(md) {
        font-size: 18px;
        line-height: 22px;
      }
      @include breakpoint(sm) {
        font-size: 16px;
        line-height: 20px;
      }
      @include breakpoint(xs) {
        font-size: 14px;
        line-height: 18px;
      }
    }
  }
  &-img {
    img {
      width: 100%;
      height: 100%;
      object-fit: contain;
    }
  }
}
</style>