<template>
  <div :class="['sidebar', { active: active }]">
    <div class="sidebar-wrapper">
      <div class="logo">
          <img src="../assets/img/logo.png" alt="" />
        </div>
      <div class="sidebar-menu">
          <div class="sidebar-menu__link">Product</div>
          <div class="sidebar-menu__link">Templates</div>
          <div class="sidebar-menu__link">Pricing</div>
          <div class="sidebar-menu__link">Customers</div>
          <div class="sidebar-menu__link">Learn</div>
        </div>
        <div class="sidebar-entry">
          <Button title="Log in" />
          <Button title="Start free trial" />
        </div>
    </div>
  </div>
</template>

<script>

import Button from '@/components/Button.vue'

export default {
  name: "Sidebar",
  components: {Button},
  props: {
    active: {
      type: Boolean,
      default: false,
    },
  },
};
</script>

<style lang="scss" scoped>
.sidebar {
  display: flex;
  position: fixed;
  top: 0;
  left: 0;
  bottom: 0;
  width: 300px;
  background: #fff;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  color: #000;
  transform: translateX(-150%);
  transition: 0.3s;
  z-index: 1000;
  @media screen and (max-width: 381px){
      width: 250px;
    }
  &.active {
    transform: translateX(0);
  }
  &-wrapper {
    display: flex;
    flex-direction: column;
    width: 100%;
    gap: 30px;
    padding: 20px;
  }
  &-menu {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  &-entry {
    display: flex;
    flex-direction: column;
    gap: 10px;
    &__btn {
      width: 94px;
      height: 54px;
      background-color: white;
      border: 2px solid #02020237;
      border-radius: 8px;
    }
    &__btn1 {
      width: 153px;
      height: 54px;
      background-color: #0099ff;
      border-radius: 8px;
      border: none;
      color: #fff;
    }
  }
}
</style>