<template>
  <h2>Technokeens</h2>
<storeResorces :resources="storedResorcesData"/>
</template>

<script>
import storeResorces from './components/learningComp/storeResorces.vue';

export default {
  components: {
    storeResorces,
},
  data() {
    return {
      storedResorcesData: [
        {
          id: "official-guide",
          title: "official guide",
          descriptions: "the official vue js documantion",
          link: "http://vuejs.org",
        },
        {
          id: "google-guide",
          title: "Google guide",
          descriptions: "the official google documantion",
          link: "http://google.org",
        },
      ],
    };
  },
  methods: {},
};
</script>

<style>
*{
  box-sizing: border-box;
}
body{
  margin: 0%;
}


</style>
