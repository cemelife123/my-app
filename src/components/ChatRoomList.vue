<template>
    <div class="chat-room-list">
      <div v-for="room in rooms" :key="room.id">
        {{ room.name }}
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ChatRoomList',
    data() {
      return {
        rooms: [
          { id: 1, name: 'General' },
          { id: 2, name: 'Random' },
          // Add more rooms as needed
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .chat-room-list {
    /* Add your styles here */
  }
  </style>
  