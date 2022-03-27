<template>
  <section class="download-page page-box">
    <div class="download-page__cards">
      <DownloadCard :image="require('~/assets/images/megadownload.png')" label="Download mega" link="#" name="Mega" />
      <DownloadCard :image="require('~/assets/images/drivedownload.png')" label="Download drive" link="#" name="Google Drive"/>
    </div>
    <div class="download-page__required">
      <h2>Requisitos</h2>
      <p>Certifique-se de que sua máquina possui os requisitos necessários para o funcionamento adequado do jogo.</p>
    </div>
  </section>
</template>

<script>
import DownloadCard from '../../components/DonwloadCard/DownloadCard.vue'
export default {
  components: { DownloadCard },

}
</script>

<style lang="scss" src="./styles.scss" />