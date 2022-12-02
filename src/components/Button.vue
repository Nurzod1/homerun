<template>
    <button >{{title}}</button>
</template>

<script>
export default {
  name: 'Button',
  props:{
    title:{
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
  button{
    display: flex;
    justify-content: center;
    border: 2px solid#02020237;
    border-radius: 12px;
    width: fit-content;
    padding: 17px 22px;
    background-color: inherit;
    color: inherit;
    @include breakpoint(md){
    padding: 12px 17px;
    }
  }
</style>