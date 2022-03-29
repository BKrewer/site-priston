<template>
  <section class="download-page page-box">
    <div class="download-page__cards">
      <DownloadCard
        :image="require('~/assets/images/megadownload.png')"
        label="Download mega"
        link="#"
        name="Mega"
      />
      <DownloadCard
        :image="require('~/assets/images/drivedownload.png')"
        label="Download drive"
        link="#"
        name="Google Drive"
      />
    </div>
    <div class="download-page__required">
      <h2>Requisitos</h2>
      <p>
        Certifique-se de que sua máquina possui os requisitos necessários para o
        funcionamento adequado do jogo.
      </p>
      <table>
        <tbody>
          <tr>
            <td>Sistema Operacional</td>
            <td>Windows Vista/7/8/10</td>
          </tr>
          <tr>
            <td>Processador</td>
            <td>Core 2 Quad 2.0</td>
          </tr>
          <tr>
            <td>Memória RAM</td>
            <td>4GB</td>
          </tr>
          <tr>
            <td>Placa de Vídeo</td>
            <td>1GB+</td>
          </tr>
          <tr>
            <td>Internet</td>
            <td>2MB</td>
          </tr>
          <tr>
            <td><b>DirectX</b></td>
            <td>9 ou Superior</td>
          </tr>
        </tbody>
      </table>
    </div>
  </section>
</template>

<script>
import DownloadCard from "../../components/DonwloadCard/DownloadCard.vue";
export default {
  components: { DownloadCard },
};
</script>

<style lang="scss" src="./styles.scss" />