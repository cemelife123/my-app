<template>
    <div id="app">
      <div class="sidebar">
        <ChannelList />
        <ChatChannel/>
        <ChatRoomList />
        <UserList />
        <DirectMessageList />
      </div>
      <div class="main">
        <ChatRoom />
        <DirectMessage />
      </div>
      <div class="input">
        <MessageInput />
      </div>
    </div>
  </template>
  
  <script>
  import ChatRoom from './components/ChatRoom.vue'
  import MessageInput from './components/MessageInput.vue'
  import ChatRoomList from './components/ChatRoomList.vue'
  import UserList from './components/UserList.vue'
  import ChatChannel from './components/ChatChannel.vue'
  import ChannelList from './components/ChannelList.vue'
  import DirectMessage from './components/DirectMessage.vue'
  import DirectMessageList from './components/DirectMessageList.vue'
  
  export default {
    name: 'App',
    components: {
      ChatRoom,
      MessageInput,
      ChatRoomList,
      UserList,
      ChatChannel,
      ChannelList,
      DirectMessage,
      DirectMessageList
    }
  }
  </script>
  
  <style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    display: flex;
    height: 100vh;
  }
  
  .sidebar {
    width: 20%;
    background-color: #2c2f33;
    color: #fff;
  }
  
  .main {
    width: 60%;
    background-color: #36393f;
    color: #dcddde;
  }
  
  .input {
    width: 20%;
    background-color: #2c2f33;
    color: #fff;
  }
  </style>
  

