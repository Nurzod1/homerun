<template>
  <div class="teams">
    <div class="container">
      <div class="teams-wrapper">
        <div class="teams-title">
          Join thousands of teams hiring with Homerun
        </div>
        <div class="teams-logos">
          <div class="teams-logos__item">
            <img src="../assets/img/Team1.png" alt="" />
          </div>
          <div class="teams-logos__item">
            <img src="../assets/img/Team2.png" alt="" />
          </div>
          <div class="teams-logos__item">
            <img src="../assets/img/Team3.png" alt="" />
          </div>
          <div class="teams-logos__item">
            <img src="../assets/img/Team4.png" alt="" />
          </div>
          <div class="teams-logos__item">
            <img src="../assets/img/Team5.png" alt="" />
          </div>
          <div class="teams-logos__item">
            <img src="../assets/img/Team6.png" alt="" />
          </div>
          <div class="teams-logos__item">
            <img src="../assets/img/Team7.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Teams",
};
</script>

<style lang="scss" scoped>
.teams {
  &-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  &-title {
    font-size: 20px;
    line-height: 28px;
    color: #b2b2b2;
    @include breakpoint(xs){
      font-size: 16px;
      line-height: 18px;
    }
  }
  &-logos {
    display: flex;
    justify-content: center;
    @include breakpoint(lg) {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr 1fr;
    }
    @include breakpoint(sm) {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
    }
    @include breakpoint(xs) {
      display: grid;
      grid-template-columns: 1fr 1fr;
    }
    @media screen and (max-width: 396px) {
      display: flex;
      flex-direction: column;
      text-align: center;
    }
    &__item:last-child {
      @include breakpoint(lg) {
        display: none;
      }
    }
  }
}
</style>