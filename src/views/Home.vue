<template>
  <div class="home">
    <Navbar />
    <Best />
    <Citys />
    <Globally />
    <Watch />
    <Our />
    <Choose />
    <Write />
    <News />
    <Finish />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Best from "@/components/Best.vue";
import Citys from "@/components/Citys.vue";
import Globally from "@/components/Globally.vue";
import Watch from "@/components/Watch.vue";
import Our from "@/components/Our.vue";
import Choose from "@/components/Choose.vue";
import Write from "@/components/Write.vue";
import News from "@/components/News.vue";
import Finish from "@/components/Finish.vue";
export default {
  name: "Home",
  components: {
    Navbar,
    Best,
    Citys,
    Globally,
    Watch,
    Our,
    Choose,
    Write,
    News,
    Finish,
  },
};
</script>
