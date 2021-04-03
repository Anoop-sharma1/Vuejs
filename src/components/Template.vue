<template>
    <div>
        <p v-html="rawHtml"></p>
        <h1>
            Template in Vue Js 
        </h1>
        <h3 v-once >{{name}}</h3>
        <h3>{{name}}</h3>
        <button v-on:click="updateText()">Click</button>
    </div>
</template>

<script>
export default {
  name: 'Template',
  data(){
      return {
          name: 'Anoop',
          a:10,
          b:20,
          rawHtml: "<h1>Raw Html</h1>"
      }
  },
  
  methods: {
      updateText() {
          this.name = 'Anoop Sharma';
      }
      
  }
};
</script>