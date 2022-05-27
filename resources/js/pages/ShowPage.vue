<template>
    <div v-if="post">
        <h1>{{ post.title }}</h1>
        <p>{{ post.description }}</p>
    </div>
</template>

<script>
export default {
    name: 'ShowPage',
    props: ['slug'],
    data () {
        return {
            post: null,
            baseUrl: 'http://127.0.0.1:8000/api/posts',
        }
    },
    created(){
        this.getArray(this.baseUrl + '/' + this.slug)
    },
    /*methods: {
        getArray(http) {
            if (http) {
                Axios.get(http)
                .then(element => {
                    if (element.data.success){
                        this.post = element.data.response.data;
                        console.log(this.post);
                    } else {
                        console.log('No');
                    }
                })
            }
        }
    }*/
    methods: {
        getArray(http) {
            if (http) {
                Axios.get(http)
                .then(element => {
                    this.post = element.data.response;
                    console.log(this.post);
                })
            }
        }
    }
    
}
</script>

<style scoped>

</style>