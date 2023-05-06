<script >

import HeaderComponent from './components/HeaderComponent.vue'

export default{
  name: 'app',
  components: {
    HeaderComponent
  }
}

</script>

<template>
  <HeaderComponent :titleProps=" 'RICK & MORTY - API exercise' "/>
</template>

<style lang="scss">
@use './style/main.scss';
</style>
