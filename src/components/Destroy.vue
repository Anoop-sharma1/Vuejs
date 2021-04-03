<template>
    <div>
        <h1>{{name}}</h1>
    </div>
</template>

<script>
export default {
    name: 'Destroy',
    data() {
        return {
            name : 'Anoop Sharma'
        }
    },
    beforeUnmount() {
        console.log('Beforedestroyed');
    },
    unmounted() {
        this.name = "Sameer";
        console.log('destroyed');
    }
}
</script>