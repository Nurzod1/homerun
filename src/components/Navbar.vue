<template>
  <div class="navbar">
    <div class="container">
      <div class="navbar-wrapper">
        <div class="logo">
          <img src="../assets/img/logo.png" alt="" />
        </div>
        <div class="navbar-menu">
          <div class="navbar-menu__link">Product</div>
          <div class="navbar-menu__link">Templates</div>
          <div class="navbar-menu__link">Pricing</div>
          <div class="navbar-menu__link">Customers</div>
          <div class="navbar-menu__link">Learn</div>
        </div>
        <div class="navbar-entry">
          <Button title="Log in" />
          <Button title="Start free trial" />
        </div>
        <Burger-menu :value="value" @input="$emit('input', $event)"/>
      </div>
    </div>
  </div>
</template>

<script>
import BurgerMenu from '@/components/BurgerMenu.vue';
import Button from "@/components/Button.vue";
export default {
  components: { Button, BurgerMenu },
  name: "Navbar",
  props: {
    value: {
      type: Boolean,
      required: true, 
    }
  },
};
</script>

<style lang="scss" scoped>
.navbar {
  &-wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px;  
  }
  &-menu {
    display: flex;
    gap: 20px;
    @include breakpoint(md){
      display: none;
    }

    &__link{
      cursor: pointer;
      transition: 0.3s;
      &:hover {
        text-shadow: 2px 2px rgba(0, 0, 0, 0.292);
      }
    }
  }
  &-entry {
    display: flex;
    gap: 10px;
    @include breakpoint(md){
      display: none;
    }
    &__btn {
      width: 94px;
      height: 54px;
      background-color: white;
      border: 2px solid #02020237;
      border-radius: 10px;
    }
    &__btn1 {
      width: 153px;
      height: 54px;
      background-color: #0099ff;
      border-radius: 10px;
      border: none;
      color: #fff;
    }
  }
  button {
    cursor: pointer;
    transition: 0.3s;
    &:hover{
      border-color: #000;
    }
  }
}
</style>