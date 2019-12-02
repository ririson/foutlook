<template>
  <div>
    <Header></Header>
    <section id="city-lists" class="section">
      <div class="container">
        <h1>日本全国の天気</h1>
        <ul>
          <li><nuxt-link :to="`city/tokyo`">東京</nuxt-link></li>
          <li><nuxt-link :to="`city/osaka`">大阪</nuxt-link></li>
          <li><nuxt-link :to="`city/fukuoka`">福岡</nuxt-link></li>
        </ul>
      </div>
    </section>
  </div>
</template>

<script>
import Header from '@/components/header.vue'

export default {
  components: {
    Header
  }
}
</script>

<style scoped>
  #city-lists {
    border: 1px solid #eeeeee;
  }
</style>
