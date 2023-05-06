<script>

import { store } from '../store';


export default {
    name: 'CharactersComponent',
    data() {
        return {
            store
        }
    },
}


</script>

<template>
    <div>
        <SingleCharacter/>
    </div>
</template>

<style lang="scss" scoped>


</style>