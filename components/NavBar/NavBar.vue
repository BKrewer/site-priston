<template>
  <nav class="navbar">
    <div class="navbar__content wrapper">
      <ul class="navbar__menu">
        <li class="navbar__link" v-for="link in links" :key="link.to">
          <NuxtLink :to="link.to">
            {{ link.name }}
          </NuxtLink>
        </li>
      </ul>
      <NuxtLink class="navbar__btn-download" to="/download'">
        Download Game
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
          name: "Home",
          to: "/",
        },
        {
          name: "Informações",
          to: "/info",
        },
        {
          name: "Guia",
          to: "/guide",
        },
      ],
    };
  },
};
</script>

<style lang="scss" src="./NavBar.scss">