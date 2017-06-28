<template>
  <img :src="loader">
  </img>
</template>

<script>
import loader from './assets/default.svg'
export default {
  data() {
    return {
      loader
    }
  }
}
</script>
