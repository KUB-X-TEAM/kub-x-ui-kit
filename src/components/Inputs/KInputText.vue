<script>
export default {
  name : "KInputText",
  props: [
      'type'
  ]
}
</script>

<template>
  <div class="k-input-text">
    <input class="" type="text" placeholder="kek">
  </div>
</template>

<style scoped>
.k-input-text input{
  outline: none;
  border: none;
  padding: 21px 20px 22px 20px;
  background-color: #000000;
  color: #ffffff;
  font-size: 15px;
}
k-input-text input::placeholder{
  font-size: 15px;
}
</style>