<template>
  <router-view name="header1"></router-view>
  <router-view></router-view>
  <router-view name="meropriyatiya"></router-view>
  <router-view name="speces"></router-view>
  <router-view name="call2action1"></router-view>
  <router-view name="opis1"></router-view>
  <router-view name="contact"></router-view>
  <router-view name="footer1"></router-view>
</template>

<script>
import { ref } from 'vue'

export default {
  setup(props) {
    let showWarn = ref(true)

    // setInterval(() => {
    //   counter.value++
    // }, 1000)

    return {
      showWarn,
    }
  },

  // components: {
  //   e1,
  //   e2,
  //   e3,
  //   e4,
  //   e5,
  //   e6,
  //   e7,
  //   e8,
  //   e9,
  //   e10,
  //   e11,
  //   e12,
  //   e13,
  //   e14,
  //   e15,
  //   e16,
  //   e17,
  //   e18,
  //   e19,

  // },
}
</script>

<style>
html {
  scroll-behavior: smooth;
}
.warning {
  position: fixed;
  top: 30%;
  left: 15%;
  right: 15%;
  background-color: yellow;
  font-weight: bold;
  text-align: center;
  padding: 20px;
}
</style>
