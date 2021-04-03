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
    },

    beforeCreate:function(){
        console.log('Before Create');
    },
    created:function(){
        console.log('Created');
    },
    beforeMount:function(){
        console.log('Before Mount');
    },
    mounted:function(){
        console.log('Mounted');
    },
}
</script>