<template>
  <div class="home">
    <div v-for="i in react" :key="i.name">
      <img :src="i.logo"  /> {{i.name}}
    </div>
  </div>
</template>

<script>
import s from "../../event"
export default {
  name: 'HomeView',
  data() {
    return {
      react: s
    }
  }
}
</script>
