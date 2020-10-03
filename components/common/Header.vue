<template>
  <header class="navbar">
    <section class="navbar__section">
      <a href="#" class="btn btn-link">Docs</a>
      <a href="#" class="btn btn-link">Examples</a>
    </section>
    <section class="navbar__center">
      <p>test</p>
    </section>
    <section class="navbar__section">
      <a href="#" class="btn btn-link">Twitter</a>
      <a href="#" class="btn btn-link">GitHub</a>
    </section>
  </header>
</template>

<script>
export default {
  data() {
    return {
      colors: ['system', 'light', 'dark', 'sepia'],
    }
  },
  methods: {
    getIcon(color) {
      switch (color) {
        case 'system':
          return 'desktop_windows'
        case 'light':
          return 'wb_sunny'
        case 'dark':
          return 'nights_stay'
        case 'sepia':
          return 'bedtime'
        default:
          return 'desktop_windows'
      }
    },
  },
}
</script>
