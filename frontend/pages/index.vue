<template>
<div>
  <v-card>
    <v-textarea @paste.prevent="paste">

    </v-textarea>
  </v-card>
</div>
</template>

<script lang="ts">
import {defineComponent} from "@nuxtjs/composition-api";

export default defineComponent({
  setup(){
    const paste = (e) => {
      console.log(e);
    };

    return {
      paste,
    }
  }
});
</script>
