<template>
    <div>
        <button v-on:click="updateTitle()">Update Parent Title</button>
    </div>
</template>

<script>
export default {
    name:'Child',
    methods: {
        updateTitle() {
            // console.log('Check');
            this.$emit('changeTitle' , "Parent Updated")
        }
    }
}
</script>