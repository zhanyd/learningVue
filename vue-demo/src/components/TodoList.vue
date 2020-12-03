<template>
     <ul>
        <todo-item v-for="item in list" :title="item.title" :key="item.title" :del="item.del"></todo-item>
    </ul>
</template>

<script>

import TodoItem from './TodoItem'

export default {
    components: {
        TodoItem
    },
    data: function() {
        return{
            list: [
                {
                    title: '课程1',
                    del: false
                },
                {
                    title: '课程2',
                    del: true
                }
            ]}
    },
    methods: {
    
    }
}
</script>