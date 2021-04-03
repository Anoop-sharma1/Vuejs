<template>
    <div>
        <h1>{{name}}</h1>
    </div>
</template>

<script>
export default {
    name: 'LifeCycle',
    data() {
        return {
            name : 'Anoop Sharma'
        }
    },
    beforeCreate() {
        console.log('beforeCreate');
    },
    created() {
        this.name = "Sameer";
        console.log('created');
    }
}
</script>