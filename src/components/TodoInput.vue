<template>
    <div>
        <input
                v-model="message"
                @keyup.enter="addTodo"
        >

        <a
                href="#"
                @click="addTodo"
        >Add</a>
    </div>
</template>

<script>
    export default {
        name: 'TodoInput',
        data(){
            return {
                message: ''
            }
        },
        methods: {
            addTodo () {
                if (!this.message) return;

                //  触发事件'add'
                this.$emit('add', this.message);
                this.message = '';
            }
        }
    }
</script>

<style></style>