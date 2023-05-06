<script>
export default {
    name: 'HeaderComponent',
    props: ['titleProps', 'classProps']
}

</script>

<template>
    <div>
        <h1 :class="classProps">{{ titleProps }}</h1>
    </div>
</template>

<style lang="scss" scoped>


</style>