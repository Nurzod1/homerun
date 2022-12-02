<template>
  <div class="create">
    <div class="container">
      <div class="create-wrapper">
        <div class="create-media">
          <div class="create-media__img">
            <img src="../assets/img/Frame2.png" alt="">
          </div>
          <div class="create-media__text">Career page created with Homerun.</div>
        </div>
        <div class="create-about">
          <div class="create-about__subtitle">Create</div>
          <div class="create-about__title">An experience candidates simply love.</div>
          <div class="create-about__text">Treat candidates with a rich career site, beautiful job posts, tailored application forms and faster response times.</div>
          <Button title="Learn more"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Button from './Button.vue'
export default {
  components: { Button },
  name: 'Create'
}
</script>

<style lang="scss" scoped>
.create{
  margin: 160px 0;
  @include breakpoint(md){
      margin: 70px 0;
    }
  &-wrapper{
    display: flex;
    gap: 20px;
    justify-content: center;
    @include breakpoint(md){
      gap: 10px;
      align-items: center;
    }
    @include breakpoint(xs){
      flex-direction: column;
      gap: 10px;
      align-items: center;
      text-align: center;
    }
  }
  &-about{
    display: flex;
    flex-direction: column;
    gap: 20px;
    @include breakpoint(md){
      gap: 10px;
    }
    @include breakpoint(xs){
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    &__subtitle{
      font-size: 30px;
      line-height: 36px;
      font-weight: 700;
      color: #0C9F64;
      @include breakpoint(md){
        font-size: 18px;
        line-height: 22px;
      }
    }
    &__title{
      font-size: 56px;
      line-height: 63px;
      font-weight: 700;
      letter-spacing: 1.5px;
      max-width: 420px;
      @include breakpoint(lg){
        font-size: 46px;
        line-height: 57px;
        letter-spacing: 1px;
      }
      @include breakpoint(md){
        font-size: 24px;
        line-height: 28px;
      }
    }
    &__text{
      font-size: 20px;
      line-height: 30px;
      max-width: 443px;
      @include breakpoint(lg){
        font-size: 16px;
        line-height: 24px;
      }
    }
  }
  &-media{
    display: flex;
    flex-direction: column;
    gap: 10px;
    text-align: center;
    &__img{
      img{
        width: 100%;
        height: 100%;
      }
    }
    &__text{
      font-size: 16px;
      line-height: 20px;
      color: #0E101666;
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