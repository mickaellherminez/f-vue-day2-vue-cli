<template>
  <div class="about">
    <HelloWorld msg="Bonjour !" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import axios from "axios";

export default {
  name: "About",
  components: {
    HelloWorld,
  },
  data() {
    return {};
  },
  methods: {},
  created() {
    axios
      .get(`http://jsonplaceholder.typicode.com/posts`)
      .then((response) => {
        // JSON responses are automatically parsed.
        console.log('response.data)', response.data);
      })
      .catch((e) => {
        console.log('e: ', e);
      });
  },

  mounted() {},
  watch: {},
};
</script>