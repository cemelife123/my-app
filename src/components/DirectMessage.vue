<template>
    <div class="direct-message">
      <h2 class="recipient">{{ recipient }}</h2>
      <MessageList :messages="messages" class="message-list" />
      <MessageInput @send="sendMessage" class="message-input" />
    </div>
  </template>
  
  <script>
  import MessageList from './MessageList.vue'
  import MessageInput from './MessageInput.vue'
  
  export default {
    name: 'DirectMessage',
    components: {
      MessageList,
      MessageInput
    },
    data() {
      return {
        recipient: 'User Name',
        messages: [] // This would be an array of messages for the direct message
      }
    },
    methods: {
      sendMessage(text) {
        // Here you would handle sending the message
        // This could involve updating the `messages` array and making a request to your server
        this.messages.push(text);
      }
    }
  }
  </script>
  
  <style scoped>
  /* Your styles... */
  </style>
  