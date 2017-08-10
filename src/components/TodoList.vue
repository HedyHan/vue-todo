
<template>
    <ul>
        <li v-for="item in items">
            {{ item.message }}
        </li>
    </ul>
</template>

<script>
    export default {
        name: 'TodoList',
        data(){
            return {
                items: [
                    {message: 'Foo' },
                    {message: 'Bar' }
                ]
            }
        }
    }
</script>

<style></style>