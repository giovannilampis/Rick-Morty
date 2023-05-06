<script>
export default {
    name: 'SingleCharacter',
    props: ['detailsCharacter']
}

</script>

<template>
    <div class="text-center col-12 col-md-6 col-lg-4">
        <img class="rounded-circle" :src="detailsCharacter.image" :alt="detailsCharacter.name">
        <h3>{{ detailsCharacter.name }}</h3>
        <span>{{ detailsCharacter.location.name }}</span>
    </div>
</template>

<style lang="scss" scoped>


</style>