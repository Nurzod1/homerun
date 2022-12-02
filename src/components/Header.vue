<template>
  <div class="header">
    <div class="container">
      <div class="header-wrapper">
        <div class="header-title">Where hiring comes together.</div>
        <div class="header-text">
          Everything you need to organise your hiring and make a great
          impression.
        </div>
        <div class="header-start">
          <input type="text" placeholder="Work email" />
          <button>Start free trial</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" scoped>
.header {
  padding: 70px 0;
  @include breakpoint(sm) {
    padding: 40px 0;
  }
  &-wrapper {
    display: flex;
    flex-direction: column;
    text-align: center;
    align-items: center;
    gap: 30px;
  }
  &-title {
    font-size: 120px;
    line-height: 110px;
    max-width: 893px;
    @include breakpoint(lg) {
      font-size: 100px;
      line-height: 90px;
    }
    @include breakpoint(md) {
      font-size: 86px;
      line-height: 76px;
    }
    @include breakpoint(sm) {
      font-size: 54px;
      line-height: 45px;
    }
    @media screen and (max-width: 410px) {
      font-size: 42px;
      line-height: 42px;
    }
  }
  &-text {
    font-size: 26px;
    line-height: 36px;
    max-width: 509px;
    @include breakpoint(md) {
      font-size: 24px;
      line-height: 32px;
    }
    @include breakpoint(sm) {
      font-size: 19px;
      line-height: 26px;
    }
    @media screen and (max-width: 410px) {
      font-size: 16px;
      line-height: 18px;
    }
  }
  &-start {
    display: flex;
    input {
      border: 2px solid #0099ff;
      border-radius: 8px 0px 0px 8px;
      width: 300px;
      height: 54px;
      color: #000;
      padding: 5px;
      font-size: 20px;
      line-height: 26px;
      outline: none;
      &::placeholder {
        color: #b2b2b2;
      }
      @include breakpoint(md) {
        height: 48px;
      }
      @include breakpoint(xs) {
        font-size: 16px;
        line-height: 20px;
        width: 200px;
      }
      @media screen and (max-width: 410px) {
        width: 150px;
      }
    }
    button {
      background-color: #0099ff;
      width: 157px;
      height: 54px;
      border-radius: 0px 8px 8px 0px;
      border: none;
      color: #fff;
      font-size: 20px;
      line-height: 25px;
      cursor: pointer;
      transition: 0.3s;
      &:hover {
      background-color: #005994;
      }
      @include breakpoint(md) {
        height: 48px;
      }
      @include breakpoint(xs) {
        font-size: 16px;
        line-height: 20px;
        width: 120px;
      }
    }
  }
}
</style>