<template>
  <nav class="navbar">
    <div class="navbar__content wrapper">
      <ul class="navbar__menu">
        <li class="navbar__link" v-for="link in links" :key="link.to">
          <a v-if="link.external" :href="link.to" rel="noopener noreferrer">{{ link.name }}</a>
          <NuxtLink v-else :to="link.to">
            {{ link.name }}
          </NuxtLink>
        </li>
      </ul>
      <NuxtLink class="navbar__btn-download" to="/download">
        Download do jogo
      </NuxtLink>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      links: [
        {
          name: "Início",
          to: "/",
        },
        {
          name: 'Conta',
          to: '#',
          external: true
        },
        {
          name: "Informações",
          to: "/info",
        },
        {
          name: "Guias",
          to: "/guide",
        },
        {
          name: "Rankings",
          to: "/rankings",
        },
        {
          name: "Suporte",
          to: "/support",
        },
      ],
    };
  },
};
</script>

<style lang="scss" src="./NavBar.scss">