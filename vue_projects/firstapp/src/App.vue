<template>
  <h1>Simple calculator</h1>
<p>
<label for="number1">Number 1:</label>
<input name="number1" v-model.number="number1" type="number">
</p>
<p>
<label for="number2">Number 2:</label>
<input name="number2" v-model.number="number2" type="number">
</p>
<button v-on:click="add">Add</button>
<button v-on:click="subtract">Subtract</button>
<p>
<label for="result">Result:</label>
<input name="result" v-model.number="result" readonly
type="number">
</p>
</template>
<script>
export default {
  name: "App" ,
  data () {
    return {
      number1: 0,
      number2: 0
      result: 0
    }
},
methods: {
  add () {
    this.result = this.number + this.number2
  },
  subtract () {
    this.result = thisnumber1 - this.number2
  }
}
}
</script>

<style>



</style>