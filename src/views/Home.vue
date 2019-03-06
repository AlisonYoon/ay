<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
    <HelloWorld
      msg="Alison Yoon is a product designer based in Bristol, UK. Her work combines
      backgrounds in graphic/web design and user-centered design. Alison
      currently works at Boxarr, where she’s responsible for all phases of
      design process from UX to UI. The Business Intelligence tool she’s
      designing here has clients such as Airbus, Deloitte UK and more."
    />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  }
}
</script>
