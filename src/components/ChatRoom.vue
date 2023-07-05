<template>
	<div class="chat-room">
	  <MessageList :messages="messages" />
	  <MessageInput @send="addMessage" />
	</div>
  </template>
  
  <script>
  import MessageList from './MessageList.vue';
  import MessageInput from './MessageInput.vue';
  
  export default {
	name: 'ChatRoom',
	components: {
	  MessageList,
	  MessageInput
	},
	data() {
	  return {
		messages: []
	  }
	},
	methods: {
	  addMessage(text) {
		this.messages.push({ text, id: Date.now() });
	  }
	}
  }
  </script>
  