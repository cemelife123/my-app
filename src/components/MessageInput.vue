<template>
    <form @submit.prevent="send">
      <input v-model="text" type="text" placeholder="Type a message" />
      <button type="submit">Send</button>
    </form>
  </template>
  
  <script>
  export default {
    name: 'MessageInput',
    data() {
      return {
        text: ''
      }
    },
    methods: {
      send() {
        this.$emit('send', this.text);
        this.text = '';
      }
    }
  }
  </script>
  