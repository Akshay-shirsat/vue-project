<template>

<ul>
<LearningResorces v-for="res in resources"
      :key="res.id"
      :title="res.title"
      :descriptions="res.descriptions"
      :link="res.link" />
  </ul>
</template>

<script>
import LearningResorces from "./LearningResorces.vue"
export default{
components:{
    LearningResorces
},
props:['resources'],
}

</script>

<style scoped>
ul{
    list-style:none;
    margin:0;
    padding:0;
    margin:auto;
    max-width:40rem;
}
</style>