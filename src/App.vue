<template>
    <div id="app">
      <ChannelList />
      <ChatChannel/>
      <ChatRoomList />
      <UserList />
      <DirectMessageList />
      <ChatRoom />
      <DirectMessage />
      <MessageInput />
    </div>
  </template>
  
  <script>
  // Import the DirectMessageList component
  import DirectMessageList from './components/DirectMessageList.vue'
  // Other imports...
  
  export default {
    name: 'App',
    components: {
      // Other components...
      DirectMessageList
    }
  }
  </script>
  
  <style>
  /* Your styles... */
  </style>
  