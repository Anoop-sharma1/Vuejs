<template>
    <div>
        <h1>DataBinding</h1>
        <h1>{{ message }}</h1>
        <textarea type="text" v-model="message" />
    </div>
</template>

<script>
export default {
    name: 'DataBinding',
    data() {
        return {
            message: "hello"
        }
    }
}
</script>