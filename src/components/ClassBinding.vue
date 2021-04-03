<template>
    <div>
        <h1 class="home-style">Class And Style Binding</h1>
        <h1 v-bind:style="{color:'blue'}">Style Binding</h1>
        <h1 v-bind:class="{display:show}">Class Binding With Object</h1>
        <h1 v-bind:class="[arrayClass]">Class Binding With Array</h1>
    </div>
</template>

<script>
export default {
    name:"ClassBinding",
    data(){
        return {
            show:true,
            arrayClass : 'array'
        }
    }
}
</script>

<style scoped>
    .home-style{
        color:goldenrod
    }

    .display{
        background-color: hotpink;
    }

    .array{
        background-color: cyan;
    }
</style>