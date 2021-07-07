<template>
  <div class="centered">
    <Hero />
    <HomeProjectBanner
      v-for="projectInfo in homePageProjects"
      :key="projectInfo.id"
      :project-home-banner="projectInfo"
    />
    <Footer />
  </div>
</template>

<script>

  import { HomeProjectBanners } from "@/assets/data.js"
  export default {
    data() {
      return {
        homePageProjects: HomeProjectBanners
      }
    }
  }

</script>

<style scoped>

</style>