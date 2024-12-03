<template>
  <ul>
    <li v-for="link in links" :key="link.url">
      <a :href="link.url" target="_blank">
        <img :src="link.icon" alt="" class="icon" />
        <span class="link-text">{{ link.name }}</span>
      </a>
    </li>
  </ul>
</template>

<script>
export default {
  name: "LinkList",
  props: {
    links: Array,
  },
};
</script>

<style scoped>
ul {
  list-style: none;
  padding: 0;
}

li {
  margin: 10px 0;
}

a {
  display: flex;
  align-items: center;
  justify-content: center; /* 使文字置中 */
  text-decoration: none;
  color: #3498db;
  font-size: 18px;
  padding: 12px;
  border: 1px solid #3498db;
  border-radius: 12px; /* 增加圓角 */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* 增加陰影 */
  transition: background-color 0.3s, color 0.3s, box-shadow 0.3s;
}

a:hover {
  background-color: #3498db;
  color: #fff;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2); /* 增加懸停時的陰影 */
}

.icon {
  width: 24px;
  height: 24px;
  margin-right: 10px;
}

.link-text {
  flex: 1; /* 使文字占據剩餘空間 */
  text-align: center; /* 使文字在其區域內置中 */
}
</style>
