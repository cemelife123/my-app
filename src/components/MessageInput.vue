<template>
    <form @submit.prevent="send" class="message-input">
      <input v-model="text" type="text" placeholder="Type a message" class="input-field"/>
      <button type="submit" class="send-button">Send</button>
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
  
  <style scoped>
  .message-input {
    background-color: #40444b;
    padding: 10px;
    display: flex;
    justify-content: space-between;
  }
  
  .input-field {
    flex-grow: 1;
    margin-right: 10px;
    padding: 5px;
    background-color: #2f3136;
    border: none;
    color: #dcddde;
  }
  
  .send-button {
    background-color: #7289da;
    color: white;
    border: none;
    padding: 5px 10px;
    cursor: pointer;
  }
  </style>
  