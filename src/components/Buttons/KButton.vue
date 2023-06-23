<script>
export default {
  name : 'KButton',
  props : [
      'color',
      'href',
      'arrow',
      'size'
  ],
  computed: {
    cls(){
      return 'k-btn ' + (this.color ? this.color : 'primary') + ' ' + (this.size ? this.size : 'default')
    }
  }
}
</script>

<template>

  <a :href="href" :class="cls" v-if="href">
    <slot></slot> <img v-if="arrow" src="@/assets/btn-arrow.svg" />
  </a>
  <button :class="cls" v-else>
    <slot></slot> <img v-if="arrow" src="@/assets/btn-arrow.svg" />
  </button>
</template>

<style scoped>
.k-btn {
  border: none;
  appearance: none;
  box-shadow: none;
  cursor: pointer;
  text-decoration: none;

  display: inline-flex;
  align-items: center;
  font-family: Arial;

  transition: 0.5s;
  color: #ffffff;
}
.k-btn.small{
  padding: 20px 28px 20px 27px;
  font-size: 15px;
}
.k-btn.default{
  padding: 30px 42px 30px 43px;
  font-size: 17px;
}
.k-btn.big{
  padding: 50px 56px 50px 54px;
  font-size: 20px;
}
.k-btn img{
  transition: 0.5s;
}
.k-btn.small img{
  width: 15px;
  height: 15px;
  margin-left: 40px;
}
.k-btn.default img{
  width: 17px;
  height: 17px;
  margin-left: 60px;
}
.k-btn.big img{
  width: 20px;
  height: 20px;
  margin-left: 80px;
}
.k-btn:hover img{
  transform: rotate(45deg);
}
.k-btn.primary{
  background-color: #FF0069;
}
.k-btn.primary:hover{
  background-color: #CE0055;
}
.k-btn.secondary{
  background-color: #09090B;
}
.k-btn.secondary:hover{
  background-color: #212123;
}
</style>