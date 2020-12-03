<template>
     <li>
        <span v-if="!del">{{title}}</span>
        <span v-else style="text-decoration: line-through;">{{title}}</span>
        <button v-show="!del">删除</button>
    </li>
</template>

<script>
export default {
    props: {
        title: String,
        del: {
            type: Boolean,
            default: false
        }
    },
    data: function() {
        return{}
    },
    methods: {
    
    }
}
</script>