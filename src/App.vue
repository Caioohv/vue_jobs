<script>
export default {
  data() {
    return {
      name: "Caio Vieira",
      status: "active",
      tasks: [`Task one`, `Task two`, `Task three`],
      link: `https://google.com`
    };
  },
};
</script>

<template>
  <h1>{{ name }}</h1>
  <p v-if="status == 'active'">User is Active</p>
  <p v-else-if="status == 'pending'">User is pending</p>
  <p v-else>User is inactive</p>

  <h3>Tasks:</h3>
  <ul>
    <li v-for="task in tasks" :key="task">{{ task }} /li></li>
  </ul>

  <a v-bind:href="link">Click for Google</a>
</template>
