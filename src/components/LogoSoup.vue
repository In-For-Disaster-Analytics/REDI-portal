<template>
  <q-div>
    <button @click="count++">You clicked me {{ count }} times.</button>
    Logo Soup goes Here
    <q-img
        v-for="(logo, index) in logos[0]"
        :key="index"
        :src="logo.logo_image"
        style="max-height: 60px; max-width: 187px; margin: 10px"
        fit="contain"
        class="flex"
      >
      </q-img>
  </q-div>
</template>

<script>
import { defineComponent, ref } from 'vue';
import logosjson from "assets/json/logos.json";

const count = ref(0)

export default defineComponent({
  name: 'LogoSoup',
  components: {},
  data() {
    return {
      logos: logosjson,
    };
  },
  setup() {
    return {};
  },
})
</script>
