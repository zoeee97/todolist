<template>
  <div id="app">
    <div class="headline">
      <h1>todos</h1>
      <input type="text" v-model="todoValue">
      <input type="text" :value="todoVal" @input="changeTodoValue">
    </div> 
    <div class="section">
        Double-click to edit a todo<br>
        Written by Evan You<br>
        Part of TodoMVC
    </div>
     <div class="bottom"></div>
  </div>
</template>
<script>
export default {
  data(){
    return {
      todoValue: "What needs to be done?",
      todoVal: ""
    }
  },
  methods: {
    changeTodoValue(newVal) {
      this.todoVal = newVal
    }
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
}
h1{
  color: rgba(228, 175, 159, 0.767);

}
</style>
