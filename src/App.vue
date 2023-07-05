<template>
    <div id="app">
      <ChatRoomList />
      <UserList />
      <ChatRoom />
      <MessageInput />
    </div>
  </template>
  
  <script>
  import ChatRoom from './components/ChatRoom.vue'
  import MessageInput from './components/MessageInput.vue'
  import ChatRoomList from './components/ChatRoomList.vue'
  import UserList from './components/UserList.vue'
  
  export default {
    name: 'App',
    components: {
      ChatRoom,
      MessageInput,
      ChatRoomList,
      UserList
    }
  }
  </script>
  
  <style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
  </style>
  