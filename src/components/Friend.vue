<template>
  <div>
    I am the template for Friend .vue
    <h1>Friend: {{ friend.name }}</h1>
    <button @click="toggleFriendDisplay">Show Details</button>
    <div v-if="detailsAreVisible">
      <p>Name: {{ friend.phone }}</p>
      <p>Email address: {{ friend.email }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Friend",
  data() {
    return {
      detailsAreVisible: false,
      friend: {
        id: "manuel",
        name: "Manuel Lorenz",
        phone: "0123 45678 90",
        email: "manuel@localhost.com",
      },
    };
  },
  methods: {
    toggleFriendDisplay() {
      this.detailsAreVisible = !this.detailsAreVisible;
    },
  },
};
</script>
