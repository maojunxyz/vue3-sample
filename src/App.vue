<template>
  <div v-bind:title="msg">{{ msg }}</div>
</template>

<script>

export default {
  name: 'App',
  data(){
    return {
      msg: "Hello world！"
    }
  }
}
</script>

<style>
</style>
