<template>
    <header>
        <router-link :to="{ name: 'home'}">Home</router-link>
        <router-link :to="{ name: 'IndexPage'}">Posts</router-link>
        <h1 class="text-center mt-3">Header</h1>
    </header>
</template>

<script>
export default {
    name: 'HeaderPage'
}
</script>

<style scoped>

</style>