<script>
export default {
  data() {
    return {
      name: "Caio Vieira",
      status: true
    };
  },
};
</script>

<template>
  <h1>{{ name }}</h1>
  <p v-if="status">User is Active</p>
</template>
