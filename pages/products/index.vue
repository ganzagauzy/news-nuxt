<template>
  <div>
     <navigation />


     <lgcarddisplay
        v-for="cardinfo in lgcardinfo.slice(0,2)"
        :key="cardinfo.id"
        :cardssection="cardinfo"
      />

  </div>
</template>

<script>
import { lgcardsections,  } from "@/assets/data.js";

import navigation from "@/components/nav.vue";
export default {
  components: { navigation },

   data() {
    return {
      lgcardinfo: lgcardsections,

    };
  },

}
</script>

<style>

</style>
