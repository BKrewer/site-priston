<template>
  <div class="error-page page-box">
    <div class="error-page__header">
      <img
        class="error-page__image"
        src="~/assets/images/bad-ata.png"
        alt="Atalanta decepcionada"
      />
    </div>
    <div class="error-page__body">
      <h2 class="error-page__title">Página não encontrada</h2>
    </div>
    <div class="error-page__footer">
      <NuxtLink class="error-page__back" to="/">Voltar para o início</NuxtLink>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.error-page {
  &.page-box {
    padding: 100px;
  }

  &__header {
    width: 100%;
    display: flex;
    justify-content: center;
  }

  &__image {
    width: 40%;
  }

  &__body {
    text-align: center;
  }

  &__title {
    margin-top: 50px;
    font-size: 28px;
    font-weight: 700;
  }

  &__footer {
    text-align: center;
    margin-top: 20px;
  }

  &__back {
    font-size: 20px;
    text-decoration: none;
    color: #666666;
    font-weight: 500;

    &:hover {
      color: #333333;
    }
  }

  @media (max-width: 767px) {
      &.page-box {
          padding: 60px 30px;
      }

      &__image {
          width: 60%;
      }

      &__title {
          font-size: 22px;
      }

      &__back {
          font-size: 16px;
      }
  }
}
</style>