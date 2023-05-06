<script >

import HeaderComponent from './components/HeaderComponent.vue'
import CharactersComponent from './components/CharactersComponent.vue'


export default{
  name: 'app',
  components: {
    HeaderComponent,
    CharactersComponent
  }
}

</script>

<template>
  <HeaderComponent :titleProps=" 'RICK & MORTY - API 🐝 CALL exercise' " :classProps=" 'text-center my-3' "/>
</template>

<style lang="scss">
@use './style/main.scss';
</style>
