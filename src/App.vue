<script setup>
import WelcomeItem from './components/WelcomeItem.vue'
import IconDocumentation from './components/icons/IconDocumentation.vue'
</script>

<template>
  <main>
    <header >
      <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />
    </header>

    <section>
      <h1>Trying  Vue</h1>

      <WelcomeItem>
        <template #icon>
          <IconDocumentation />
        </template>
        <template #default>Quick Start Docs</template>
        <template #heading>
          Start learning vue
        </template>
      </WelcomeItem>
    </section>
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}
main{
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  margin: 0 auto;
  width: 100%;
}
.logo {
  display: block;
  margin: 0 auto 2rem;
}
</style>
