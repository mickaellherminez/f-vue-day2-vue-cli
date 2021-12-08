<template>
  <div>
      <hello-world msg="Bonjour à tout le monde !" />
    <p>{{ $t("TO_DO_LIST") }}</p>
  </div>
</template>

<script>
  import HelloWorld from '../components/HelloWorld'

  export default {
    name: 'Home',

    components: {
      HelloWorld,
    },
    mounted () {
      console.log('trad: ', this.$i18n.t("TO_DO_LIST"))
      this.$i18n.locale = "fr";
    },
    beforeCreate () {
      
    },

  }
</script>
