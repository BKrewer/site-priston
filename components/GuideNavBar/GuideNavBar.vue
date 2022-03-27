<template>
  <nav class="guide-navbar">
    <ul class="guide-navbar__menu">
      <li class="guide-navbar__link" v-for="link in links" :key="link.to">
        <NuxtLink :to="link.to">
          {{ link.name }}
        </NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      links: [
          {
              to: '/guide/maps',
              name: 'Mapas'
          },
          {
              to: '/guide/monsters',
              name: 'Monstros'
          },
          {
              to: '/guide/item-list',
              name: 'Lista de Itens'
          },
          {
              to: '/guide/aging',
              name: 'Aging'
          },
          {
              to: '/guide/mixing',
              name: 'Mixing'
          },
      ],
    };
  },
};
</script>

<style lang="scss" src="./GuideNavBar.scss" />