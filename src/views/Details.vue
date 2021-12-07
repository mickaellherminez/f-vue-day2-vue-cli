<template>
  <div class="about">
    <HelloWorld :msg="`Bonjour ${ name }`"/> 
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Details',
  data() {
    return {
      name: this.$route.params.name
    }
  },
  components: {
    HelloWorld
  }
}
</script>