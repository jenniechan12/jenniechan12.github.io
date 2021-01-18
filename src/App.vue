<template lang="pug">
  v-app.backgroundColor
    v-app-bar(app flat color='#eb6b6f' dark)
      v-btn.ml-2(icon)
        v-img(src='./assets/logo-color.png' width='40px' height='40px')
      v-spacer
      v-btn(text color='#fff6d3' rounded @click='openContactModal = true') Say Hello
    v-main
      Contact(:openContactModal.sync='openContactModal')
      Skills
      RecentWorks
      Footer
</template>

<script>
import Footer from "./components/footer";
import Contact from "./components/contact";
import Skills from "./components/skills";
import RecentWorks from "./components/recentWorks";

export default {
  name: "App",

  components: {
    Footer,
    Contact,
    Skills,
    RecentWorks,
  },

  data() {
    return {
      openContactModal: false,
    };
  },
};
</script>
<style scoped>
.backgroundColor {
  background-color: #fff6d3 !important;
}
</style>
