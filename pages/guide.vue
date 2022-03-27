<template>
  <section class="guide-page page-box">
      <div class="guide-page__header">
        <GuideNavBar />
      </div>
      <div class="guide-page__body">
        <NuxtChild  />
      </div>
  </section>
</template>

<script>
import ComingSoon from '../components/ComingSoon/ComingSoon.vue'
import GuideNavBar from '../components/GuideNavBar/GuideNavBar.vue'
export default {
  components: { ComingSoon, GuideNavBar },
}
</script>

<style lang="scss" src="./guide/styles.scss" />