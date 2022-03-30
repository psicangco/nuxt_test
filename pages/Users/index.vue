<template>
    <div>
        <input type="text" v-model="userId">
        <button @click="onLoadUser">Create User</button>
    </div>
</template>
<script>
    export default 
    {
        data(){
            return {
                userId: ''
            }
        },
        methods: {
            onLoadUser()
            {
                this.$router.push('/Users/'+this.userId)
            }
        }
    }
</script> 