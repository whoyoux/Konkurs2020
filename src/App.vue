<template>
  <div id="app" class="flex flex-col h-screen justify-between">
    <Header />
    <router-view/>
    <footer class='w-full text-center border-t border-grey p-4 pin-b'>
            Site by <a href="https://github.com/whoyoux" target="_blank">whoyoux</a>
    </footer>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
export default {
  name: 'App',
  components: {
    Header
  }
}
</script>
