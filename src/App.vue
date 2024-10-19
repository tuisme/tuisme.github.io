<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <HelloWorld msg="Vite + Vue" />
  <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "WebSite",
      "name": "Your Website Name",
      "url": "https://www.yourwebsite.com",
      "potentialAction": {
        "@type": "SearchAction",
        "target": "https://www.yourwebsite.com/search?q={search_term_string}",
        "query-input": "required name=search_term_string"
      }
    }
  </script>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
