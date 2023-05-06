<script>

import { store } from '../store';
import SingleCharacter from './SingleCharacter.vue'

export default {
    name: 'CharactersComponent',
    components: {
        SingleCharacter
    },
    data() {
        return {
            store
        }
    },
}


</script>

<template>
    <div>
        <SingleCharacter v-for="(element, index) in store.arrayCharacters"
        :key="index"/>
    </div>
</template>

<style lang="scss" scoped>


</style>