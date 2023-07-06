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

<style scoped>
.message-list {
  height: 100%;
  overflow-y: auto;
  padding: 10px;
  text-align: left;
  background-color: #36393f;
  color: #dcddde;
}

.message-list::-webkit-scrollbar {
  width: 8px;
}

.message-list::-webkit-scrollbar-thumb {
  background-color: #202225;
  border-radius: 4px;
}

.message-list::-webkit-scrollbar-track {
  background-color: #2f3136;
}
</style>
