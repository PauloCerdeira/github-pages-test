<template>
  <div class="hello">
    <input type="number" v-model="num1" >
    <br>
    +
    <br>
    <input type="number" v-model="num2">
    <br>
    <button @click="res = parseInt(num1) + parseInt(num2)">
    =
    </button>
    <br>
    <span v-if="res != null">
      {{res}}
    </span>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      num1: 0,
      num2: 0,
      res: null
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
