<template>
    <ListUser v-for="(user, i) of users" :user="user" :key="i"></ListUser>
</template>

<script>
import axios from 'axios'
import ListUser from './listUser.vue';
    export default {
    data() {
        return {
            users: {},
        };
    },
    created() {
        this.loadUser();
    },
    methods: {
        loadUser() {
            axios
                .get("https://randomuser.me/api/?results=5")
                .then((response) => (this.users = response.data.results));
        },
    },
    components: { ListUser }
}
</script>

<style scoped>

</style>