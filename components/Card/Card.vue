<template>
  <div class="card">
      <div class="card__header">
          <h2 class="card__title">{{ title }}</h2>
          <img v-if="icon" :src="icon" class="card__icon"/>
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
        },
        icon: {
            type: String,
            default: ''
        }
    }
}
</script>

<style lang="scss" src="./Card.scss">