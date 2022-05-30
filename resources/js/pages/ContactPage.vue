<template>
    <div>
        <h1 class="text-center">Contacts</h1>
        <form  @submit.prevent="SendMessage" action="api/contact" method="post">
            <div class="mb-3">
                <label for="name" class="form-label"><h4>Name</h4></label>
                <input type="text" name="name" class="form-control" id="creator" v-model="name">
            </div>

            <div class="mb-3">
                <label for="email" class="form-label"><h4>Email</h4></label>
                <input type="text" name="email" class="form-control" id="creator" v-model="email">
            </div>

            <div class="mb-3">
                <label for="description" class="form-label"><h4>Message</h4></label>
                <textarea type="text" name="description" class="form-control" id="creator" v-model="message"></textarea>
            </div>
            <button class="btn btn-primary">Send</button>
        </form>
    </div>
</template>

<script>
export default {
    name: 'ContactPage'
}
</script>

<style scoped>

</style>