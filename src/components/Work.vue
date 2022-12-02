<template>
  <div class="work">
    <div class="container">
      <div class="work-wrapper">
        <div class="work-title">How Homerun works</div>
        <div class="work-video">
          <img src="../assets/img/Rectangle.png" alt="">
        </div>
        <button class="work-btn">
          <img src="../assets/img/Artboard.png" alt="">
          <p>Watch: Homerun in 90 seconds</p>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Work'
}
</script>

<style lang="scss" scoped>
.work{
  margin: 50px 0;
  &-wrapper{
    display: flex;
    flex-direction: column;
    gap: 30px;
    text-align: center;
    align-items: center;
  }
  &-title{
    font-size: 36px;
    line-height: 56px;
    letter-spacing: 1.5px;
    @include breakpoint(md){
      font-size: 28px;
      line-height: 36px;
      letter-spacing: 1px;
    }
  }&-video{
    img{
      width: 100%;
      height: 100%;
    }
  }
  &-btn{
    width: 361px;
    height: 70px;
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    background: #fff;
    border: none;
    border-radius: 40px;
    margin: -70px 0px 0px 0px;
    cursor: pointer;
    transition: 0.3s;
    &:hover{
      box-shadow: rgba(255, 255, 255, 0.1) 0px 1px 1px 0px inset, rgba(50, 50, 93, 0.25) 0px 50px 100px -20px, rgba(0, 0, 0, 0.3) 0px 30px 60px -30px;
    }
    @include breakpoint(sm){
      width: 261px;
      height: 50px;
      margin: -60px 0px 0px 0px;
    }
    @include breakpoint(sm){
      width: 191px;
      height: 40px;
      margin: -55px 0px 0px 0px;
      padding-left: 10px;
    }
    p{
      font-size: 18px;
      line-height: 20px;
      @include breakpoint(sm){
      font-size: 12px;
      line-height: 18px;
    }
    }
  }
}
</style>