<template>
    <div class="message-list">
      <ChatMessage v-for="message in messages" :key="message.id" :text="message.text" />
    </div>
  </template>
  
  <script>
  import ChatMessage from './ChatMessage.vue';
  
  export default {
    name: 'MessageList',
    components: {
      ChatMessage
    },
    props: {
      messages: Array
    }
  }
  </script>  