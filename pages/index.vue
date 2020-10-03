<template>
  <div>
    <Header />
    <div class="container">
      <p>
        <Logo />
      </p>
      <ThemePicker />
    </div>
  </div>
</template>

<script>
import Logo from '@/components/Logo'
import ThemePicker from '@/components/ui/ThemePicker'
import Header from '@/components/common/Header'

export default {
  components: {
    Logo,
    ThemePicker,
    Header,
  },
  head: {
    title: 'Demo of @nuxtjs/color-mode',
    meta: [
      { charset: 'utf-8' },
      { name: 'viewport', content: 'width=device-width, initial-scale=1' },
      {
        hid: 'description',
        name: 'description',
        content:
          'Demo of using @nuxtjs/color-mode for NuxtJS, supporting dark mode and custom colors',
      },
    ],
  },
}
</script>

<style scoped>
p {
  padding: 20px 0;
  margin: 0;
}

.container {
  text-align: center;
  padding: 50px;
}

.note {
  transition: all 0.3s;
  display: inline-block;
  padding: 15px 15px;
  border-radius: 5px;
  background-color: var(--bg-secondary);
  color: var(--color-secondary);
}
</style>
