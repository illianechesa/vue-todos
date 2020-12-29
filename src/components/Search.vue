<template>
    <div id="search-container">
        <h2 style="color: white; text-align: center">To-Do Application</h2>
        <input placeholder="Search for tasks..." type="text" v-model="query" v-on:input="$emit('query-change', query)">
    </div>
</template>

<script>
export default {
    name: 'Search',
    data(){
        return {
            query: ''
        }
    }
}
</script>

<style scoped>
    #search-container{
        width: 600px;
        margin: 0 auto;
    }
    input{
        padding: 10px;
        width: 100%;
        outline: none;
    }
</style>