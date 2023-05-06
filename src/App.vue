<script >

import axios from 'axios';
import HeaderComponent from './components/HeaderComponent.vue';
import CharactersComponent from './components/CharactersComponent.vue';

export default{
  name: 'app',
  components: {
    HeaderComponent,
    CharactersComponent
  },
  created() {
    callApi()
  },
}
methods: {
  callApi() {
    axios.get( 'https://rickandmortyapi/api/character' ).then( (response) =>{

    } )
  }
}

</script>

<template>

  <HeaderComponent :titleProps=" 'RICK & MORTY - API 🐝 CALL exercise' " :classProps=" 'text-center my-3' "/>

  <main class="container">

      <CharactersComponent/>

  </main>


</template>

<style lang="scss">
@use './style/main.scss';
</style>
