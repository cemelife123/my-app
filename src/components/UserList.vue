<template>
    <div class="user-list">
      <div class="user" v-for="user in users" :key="user.id">
        {{ user.name }}
      </div>
    </div>
</template>

<script>
export default {
  name: 'UserList',
  data() {
    return {
      users: [
        { id: 1, name: 'User1' },
        { id: 2, name: 'User2' },
        // Add more users as needed
      ]
    }
  }
}
</script>

<style scoped>
.user-list {
  background-color: #2f3136;
  padding: 10px;
}

.user {
  color: #dcddde;
  margin-bottom: 10px;
}
</style>
