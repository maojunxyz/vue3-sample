<template>
  <div v-if="seen" :title="msg" v-on:click="handleClick">
    {{ msg }}
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      msg: "Hello world！",
      seen: true
    }
  },
  methods: {
    handleClick() {
      this.seen = false;
    }
  }
}
</script>

<style></style>
