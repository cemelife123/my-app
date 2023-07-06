<template>
    <div class="ChatChannel">
      <h2>{{ channelName }}</h2>
      <MessageList :messages="messages" />
    </div>
  </template>
  
  <script>
  import MessageList from './MessageList.vue'
  
  export default {
    name: 'ChatChannel',
    components: {
      MessageList
    },
    data() {
      return {
        channelName: 'Channel Name',
        messages: [] // This would be an array of messages for the channel
      }
    }
  }
  </script>
  
  <style scoped>
  .ChatChannel {
    background-color: #36393F;
    color: #DCDDDE;
    width: calc(100vw - 200px); /* Assuming your channel list is 200px wide */
    height: 100vh;
    padding: 20px;
    overflow-y: auto;
  }
  
  .ChatChannel h2 {
    color: #8E9297;
    margin-bottom: 20px;
  }
  </style>
  