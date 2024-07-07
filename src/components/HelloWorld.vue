<template>
  <div v-if="seen" :title="msg" v-on:click="handleClick">
    {{ msg }}
    <template v-for="todo in todos" :key="todo">
      <div>
        {{ todo }}
      </div>
    </template>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      msg: "Hello world！",
      seen: true,
      todos: ["Vue", "React", "Angular"]
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
