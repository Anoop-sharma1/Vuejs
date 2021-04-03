<template>
    <div>
        <h1>{{name}}</h1>
    </div>
</template>

<script>
export default {
    name: 'Mounted',
    data() {
        return {
            name : 'Anoop Sharma'
        }
    },
    beforeMount() {
        console.log('beforeMounted');
    },
    mounted() {
        this.name = "Sameer";
        console.log('mounted');
    }
}
</script>