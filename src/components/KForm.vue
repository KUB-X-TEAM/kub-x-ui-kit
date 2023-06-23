<script>
  export default {
    name : "KForm",
  }
</script>

<template>
  <form class="k-form" action="">
    <slot></slot>
  </form>
</template>

<style scoped>
.k-form{
  background-color: #09090B;
  padding: 65px;
  width: fit-content;
}
</style>