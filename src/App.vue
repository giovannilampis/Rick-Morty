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
    // data(){
    //   return{
    //     store
    //   }
    // },
    created(){
      this.callApi()
    },
    methods: {
      callApi() {
        axios.get( 'https://rickandmortyapi.com/api/character' )
          .then( (response) =>{
              console.log(response.data.results)
        } )
      }
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
