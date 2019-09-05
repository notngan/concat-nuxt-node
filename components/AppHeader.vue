<template>
<header class="header">
  <CcLogo class="header__logo" />
  <nav class="header__navbar">
    <ul>
      <li><nuxt-link to="/">feed</nuxt-link></li>
      <li><nuxt-link to="/frontend">frontend</nuxt-link></li>
      <li><nuxt-link to="/backend">backend</nuxt-link></li>
      <li><nuxt-link to="/design">design</nuxt-link></li>
      <li><nuxt-link to="/user/notngan">@ngan</nuxt-link></li>
    </ul>
  </nav>
</header>
</template>
<script>
import CcLogo from '@/components/elements/CcLogo'

export default {
  components: {
    CcLogo
  }
}
</script>
