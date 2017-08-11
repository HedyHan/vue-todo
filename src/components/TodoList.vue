
<template>
    <div>
        <TodoInput v-on:add="addTodo"></TodoInput>
        <ul >
            <li v-for="item in items">
                <input type="checkbox" >
                <label>{{ item.text  }}</label>
            </li>
        </ul>
        <p>共 <strong>{{ this.items.length }}</strong> 个待办事项。</p>
    </div>
</template>

<script>
    import TodoInput from "./TodoInput.vue";

    export default {
        name: 'TodoList',
        components: {
            TodoInput
        },
        data: () => ({
            items: [
                {
                    text: 'Demo'
                }
            ]
        }),
        methods: {
            addTodo (item) {
                this.items.push({
                    text: item
                })
            }
        }
    }
</script>

<style>
    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }
</style>