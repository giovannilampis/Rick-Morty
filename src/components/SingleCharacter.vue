<script>
export default {
    name: 'SingleCharacter',
    props: ['detailsCharacter']
}

</script>

<template>
    <div class="card">
        <img :src="detailsCharacter.image" :alt="detailsCharacter.name">
        <h3>{{ detailsCharacter.name }}</h3>
    </div>
</template>

<style lang="scss" scoped>


</style>