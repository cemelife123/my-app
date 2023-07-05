<template>
  <div class="chat-message">
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  name: 'ChatMessage',
  data() {
    return {
      message: 'Hello, world!'
    }
  }
}
</script>

<style scoped>
.chat-message {
  color: blue;
}
</style>
