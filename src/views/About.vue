<template>
  <div class="about">
    <HelloWorld msg="Bonjour !"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'About',
  components: {
    HelloWorld
  },
  data() {
    return {
    }
  },
  methods: {
  },
  mounted () {
  },
  watch: {
  },
}
</script>