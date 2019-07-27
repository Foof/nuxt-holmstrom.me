<template>
  <nav class="navbar is-white">
    <div class="container">
      <div class="navbar-brand">
        <a href="/" class="navbar-item">
          {{ brand }}
        </a>
        <span class="navbar-burger burger" :class="{ 'is-active': showMobileNav }" @click="toggleNav">
          <span />
          <span />
          <span />
        </span>
      </div>
      <div class="navbar-menu" :class="{ 'is-active': showMobileNav }">
        <div class="navbar-end">
          <!-- <nuxt-link to="/kontakta" class="navbar-item">
            Kontakta
          </nuxt-link> -->
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  props: {
    brand: {
      required: true,
      type: String
    }
  },

  data () {
    return {
      showMobileNav: false
    }
  },

  methods: {
    toggleNav () {
      this.showMobileNav = !this.showMobileNav
    }
  }
}
</script>
