<template>
  <div class="reviews">
    <div class="container">
      <div class="reviews-wrapper">
        <div class="reviews-card">
          <div class="reviews-card__logo">
            <img src="../assets/img/logo3.png" alt="" />
          </div>
          <div class="reviews-card__grade">4,5</div>
          <div class="reviews-card__stars">
            <img src="../assets/img/stars.svg" alt="" />
          </div>
          <div class="reviews-card__text">
            Average review on Capterra, independent review site
          </div>
        </div>
        <div class="reviews-card">
          <div class="reviews-card__logo">
            <img src="../assets/img/logo4.png" alt="" />
          </div>
          <div class="reviews-card__grade">98,8%</div>
          <div class="reviews-card__stars"></div>
          <div class="reviews-card__text">
            Average rating based on 1500+ support conversations
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Review",
};
</script>

<style lang="scss" scoped>
.reviews {
  margin: 100px 0;
  @include breakpoint(md) {
    margin: 60px 0;
  }
  &-wrapper {
    display: flex;
    justify-content: space-evenly;
    @include breakpoint(sm) {
      flex-direction: column;
      align-items: center;
      gap: 40px;
    }
  }
  &-card {
    display: flex;
    flex-direction: column;
    gap: 20px;
    text-align: center;
    @include breakpoint(sm) {
      gap: 10px;
    }
    &__grade {
      font-size: 82px;
      line-height: 114px;
      font-weight: 700;
      @include breakpoint(sm) {
        font-size: 64px;
        line-height: 86px;
      }
    }
    &__stars {
      height: 47px;
      img {
        width: 100%;
        height: 100%;
      }
      @include breakpoint(xs) {
        height: 37px;
      }
    }
    &__text {
      font-size: 20px;
      line-height: 28px;
      max-width: 263px;
      @include breakpoint(sm) {
        font-size: 18px;
        line-height: 24px;
      }
      &:first-child {
        max-width: 254px;
      }
    }
  }
}
</style>