<template>
    <div class="direct-message-list">
      <DirectMessage v-for="dm in directMessages" :key="dm.id" :dm="dm" />
    </div>
  </template>
  
  <script>
  import DirectMessage from './DirectMessage.vue'
  
  export default {
    name: 'DirectMessageList',
    components: {
      DirectMessage
    },
    data() {
      return {
        directMessages: [
          // This would be an array of direct messages
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  /* Add your CSS styles here */
  </style>
  