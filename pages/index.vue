<template>
  <div>
    <navigation />

    <div class="container">

      <lgcarddisplay
        v-for="cardinfo in lgcardinfo.slice(0,2)"
        :key="cardinfo.id"
        :cardssection="cardinfo"
      />


    </div>
  </div>
</template>

<script>
import { lgcardsections, smcardsections } from "@/assets/data.js";

import navigation from "../components/nav.vue";

export default {
  components: {  navigation },

  data() {
    return {
      lgcardinfo: lgcardsections,

    };
  },
};
</script>
<style  scoped>


</style>


