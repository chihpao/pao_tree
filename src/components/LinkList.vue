<template>
  <div class="link-list-container">
    <header>
      <h1>{{ title }}</h1>
      <p>{{ description }}</p>
    </header>
    <ul>
      <li v-for="link in links" :key="link.url">
        <a :href="link.url" target="_blank">
          <img :src="link.icon" alt="" class="icon" />
          <span class="link-text">{{ link.name }}</span>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "LinkList",
  props: {
    title: String,
    description: String,
    links: Array,
  },
};
</script>
