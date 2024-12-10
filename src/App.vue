<template>
  <div class="container">
    <LinkList
      title="Pao"
      description="Cat, Podcast, Front-End Developer"
      :links="links"
    />
  </div>
</template>

<script>
import LinkList from "./components/LinkList.vue";

export default {
  components: {
    LinkList,
  },
  data() {
    return {
      links: [
        {
          name: "Stupid Cat",
          url: "https://funnywebsitegoodapi.vercel.app/",
          icon: require("./assets/stupidcat_icon.png"),
        },
        {
          name: "學習筆記分享",
          url: "https://chihpao.notion.site/",
          icon: require("./assets/notion_icon.png"),
        },
        {
          name: "在咖啡廳轉生成為冰美",
          url: "https://open.spotify.com/show/2gMSpNkgeKlE2Nyu8Ru4gw",
          icon: require("./assets/spotify_icon.png"),
        },
        {
          name: "Pao GitHub",
          url: "https://github.com/chihpao",
          icon: require("./assets/github_icon.png"),
        },
        {
          name: "LinkedIn",
          url: "https://www.linkedin.com/in/chihpao-chang-1745a423a",
          icon: require("./assets/linkedin_icon.png"),
        },
        {
          name: "Facebook",
          url: "https://www.facebook.com/chihpaoo",
          icon: require("./assets/facebook_icon.png"),
        },
        // 添加更多連結
      ],
    };
  },
};
</script>

<style scoped>
/* 這裡不需要任何樣式，所有樣式都在 global.css 中 */
</style>
