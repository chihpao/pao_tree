<template>
  <div class="container">
    <LinktreeHeader title="Pao" description="Cat,Podcast,Front-End Developer" />
    <LinkList :links="links" />
  </div>
</template>

<script>
import LinktreeHeader from "./components/LinktreeHeader.vue";
import LinkList from "./components/LinkList.vue";

export default {
  components: {
    LinktreeHeader,
    LinkList,
  },
  data() {
    return {
      links: [
        {
          name: "Stupid Cat",
          url: "https://funnywebsitegoodapi.vercel.app/",
          icon: require("../src/assets/stupidcat_icon.png"),
        },
        {
          name: "GitHub",
          url: "https://github.com/chihpao",
          icon: require("../src/assets/github_icon.png"),
        },
        {
          name: "LinkedIn",
          url: "www.linkedin.com/in/chihpao-chang-1745a423a",
          icon: require("../src/assets/linkedin_icon.png"),
        },
        {
          name: "Facebook",
          url: "https://www.facebook.com/chihpaoo",
          icon: require("../src/assets/facebook_icon.png"),
        },
        {
          name: "Notion",
          url: "https://chihpao.notion.site/",
          icon: require("../src/assets/notion_icon.png"),
        },
        // 添加更多連結
      ],
    };
  },
};
</script>

<style scoped>
/* 這裡可以保留特定於 App.vue 的樣式 */
</style>
