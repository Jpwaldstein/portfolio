<template lang="html">
  <aside id="side-nav" class="menu column is-one-quarter is-hidden-mobile">
    <div class="side-nav">
      <p class="menu-label">
        About
      </p>
      <ul class="menu-list">
        <nuxt-link to="/about">Me</nuxt-link>
      </ul>
      <p class="menu-label">
        Portfolio
      </p>
      <ul class="menu-list">
        <li><nuxt-link to="/portfolio/websites">Websites</nuxt-link></li>
        <li><nuxt-link to="/portfolio/plugins">Plugins</nuxt-link></li>
      </ul>
    </div>
    <Footer />
  </aside>
</template>

<script>
import Footer from "~/components/Footer.vue";

export default {
  components: {
    Footer,
  },
};
</script>

<style lang="css">
#side-nav {
  position: fixed;
  top: 75px;
  bottom: 0;
  overflow-y: scroll;
  padding-left: 25px;
}
</style>
<style lang="css" scoped>
a.nuxt-link-active {
  background-color: #00c4a7;
  color: #fff;
}
</style>
