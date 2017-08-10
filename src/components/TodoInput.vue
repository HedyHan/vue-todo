<template>
    <div>
        <input v-model="message">
    </div>
</template>

<script>
    export default {
        name: 'TodoInput',
        data(){
            return {
                message: ''
            }
        }
    }
</script>

<style></style>