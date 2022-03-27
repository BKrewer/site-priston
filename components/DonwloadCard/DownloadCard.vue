<template>
  <div class="download-card">
    <div class="download-card__header">
      <img class="download-card__image" :src="image" :alt="label" />
    </div>
    <div class="download-card__body">
        <p class="download-card__name">{{ name }}</p>
        <a class="download-card__btn-download" :href="link" target="_blank" rel="noopener noreferrer">Download</a>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    image: {
      type: String,
      default: "",
    },
    label: {
      type: String,
      default: "",
    },
    name: {
      type: String,
      default: "",
    },
    link: {
      type: String,
      default: "",
    },
  },
};
</script>

<style lang="scss" src="./DownloadCard.scss" />