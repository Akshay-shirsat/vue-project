<template>
    test
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

<style>

</style>