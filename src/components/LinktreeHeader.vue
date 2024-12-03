<template>
  <header>
    <h1>{{ title }}</h1>
    <p>{{ description }}</p>
  </header>
</template>

<script>
export default {
  name: "LinktreeHeader",
  props: {
    title: String,
    description: String,
  },
};
</script>

<style scoped>
header {
  margin-bottom: 20px;
}
</style>
