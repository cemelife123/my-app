<template>
    <div class="channel-list">
      <h2>Channels</h2>
      <ul>
        <li v-for="channel in channels" :key="channel.id">
          {{ channel.name }}
        </li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ChannelList',
    data() {
      return {
        channels: [
          { id: 1, name: 'Channel 1' },
          { id: 2, name: 'Channel 2' },
          // Add more channels as needed
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .channel-list {
    background-color: #2C2F33;
    color: #FFFFFF;
    width: 200px;
    height: 100vh;
    padding: 20px;
  }
  
  .channel-list h2 {
    color: #8E9297;
    margin-bottom: 10px;
  }
  
  .channel-list ul {
    list-style-type: none;
    padding: 0;
  }
  
  .channel-list li {
    padding: 10px 0;
    cursor: pointer;
  }
  
  .channel-list li:hover {
    color: #7289DA;
  }
  </style>
  
  