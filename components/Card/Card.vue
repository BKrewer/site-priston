<template>
  <div class="card">
      <div class="card__header">
          <h2 class="card__title">{{ title }}</h2>
          <i class="card__icon"></i>
      </div>
      <div class="card__body">
          <slot></slot>
      </div>
  </div>
</template>

<script>
export default {
    props: {
        title: {
            type: String,
            default: '',
        }
    }
}
</script>

<style lang="scss" src="./Card.scss">