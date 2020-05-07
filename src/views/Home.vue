<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <foot></foot>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import foot from '../components/footer.vue'
import Vue from 'vue'
Vue.component('footer')

export default {
  name: 'Home',
  components: {
    HelloWorld,foot

  }
}
</script>
