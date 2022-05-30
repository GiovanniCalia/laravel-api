<template>
    <header class="text-center my-3">
        <router-link :to="{ name: 'home'}" class="btn btn-dark">Home</router-link>
        <router-link :to="{ name: 'IndexPage'}" class="btn btn-dark">See Posts</router-link>
        <router-link :to="{ name: 'AboutUs'}" class="btn btn-dark">About us</router-link>
        <router-link :to="{ name: 'ContactPage'}" class="btn btn-dark">Contacts</router-link>
    </header>
</template>

<script>
export default {
    name: 'HeaderPage'
}
</script>

<style scoped>

</style>