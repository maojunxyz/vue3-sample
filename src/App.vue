<template>
  <div :title="msg" v-on:click="handleClick">{{ msg }}</div>
</template>

<script>

export default {
  name: 'App',
  data(){
    return {
      msg: "Hello world！"
    }
  },
  methods:{
    handleClick(event){
      alert(event.target.title);
    }
  }
}
</script>

<style>
</style>
