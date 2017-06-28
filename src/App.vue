<template>
  <AsyncComp>
  </AsyncComp>
</template>

<script>
const hello = () => import('./hello.vue')
import loader from './loader.vue'
const AsyncComp = () => ({
  // The component to load. Should be a Promise
  component: hello,
  // A component to use while the async component is loading
  loading: loader,
  delay: 200
})


export default {
  name: 'app',
  components: { hello, loader, AsyncComp }
}
</script>
