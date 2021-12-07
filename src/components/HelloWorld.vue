<template>
  <h1>{{msg}}</h1>
</template>

<script>
  export default {
    name: 'HelloWorld',
    data: () => ({

    }),
    props: {
      msg: {
        type: String
      },
    },
  }
</script>
