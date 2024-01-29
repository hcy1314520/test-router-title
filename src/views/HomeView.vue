<template>
  <main>
    <h3 @click="toLink">to about</h3>
  </main>
</template>

<script setup lang="ts">
import { useRouter } from 'vue-router'

const router = useRouter()

const toLink = () => {
  router.push({
    path: '/about',
    query: {
      a: '12 44'
    }
  })
}
</script>
