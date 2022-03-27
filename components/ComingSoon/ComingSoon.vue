<template>
  <div class="coming-soon">
      <div class="coming-soon__header">
          <img class="coming-soon__image" src="~/assets/images/comming.png" alt="Pike e hopi construindo" >
      </div>
      <div class="coming-soon__body">
          <h2 class="coming-soon__title">Página em construção</h2>
      </div>
      <div class="coming-soon__footer">
          <NuxtLink class="coming-soon__back" to="/" >Voltar para o início</NuxtLink>
      </div>
  </div>
</template>

<script>
export default {
    name: "ComingSoon"
}
</script>

<style lang="scss" src="./ComingSoon.scss" />