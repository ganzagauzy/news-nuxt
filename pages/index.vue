<template>
  <div>
    <navigation />

    <div class="container">
      <hero />
      <lgcarddisplay
        v-for="cardinfo in lgcardinfo.slice(0,2)"
        :key="cardinfo.id"
        :cardssection="cardinfo"
      />

      <smcarddisplay
        v-for="cardinfo in smcardsections"
        :key="cardinfo.id"
        :cardsection="cardinfo"
      />
    </div>
  </div>
</template>

<script>
import { lgcardsections, smcardsections } from "@/assets/data.js";
import smcarddisplay from "../components/smcarddisplay.vue";
import navigation from "../components/nav.vue";

export default {
  components: { smcarddisplay, navigation },

  data() {
    return {
      lgcardinfo: lgcardsections,
      smcardsections,
    };
  },
};
</script>
<style  scoped>


</style>


