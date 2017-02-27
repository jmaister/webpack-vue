<template lang="html">
<div id="app">
    <img src="./assets/logo.png">
    <h1>Vue application</h1>
    <audio src="./assets/ding.ogg" type="audio/ogg"></audio>

    <audio src="./assets/test.mp3" type="audio/mpeg"></audio>

    <audio controls>
     <source src="./assets/test.mp3" type="audio/mpeg">
     Your browser does not support the audio tag.
   </audio>

    <h2>Test component</h2>
    <hello-world></hello-world>
    <hello-world name="Jordi"></hello-world>
</div>
</template>

<script lang="js">
import HelloWorld from './HelloWorld.vue';

export default {
    name: 'app',
    data() {
        return {
            msg: 'Welcome to Your Vue.js App'
        }
    },
    components: {
        'hello-world': HelloWorld
    }
}
</script>

<style lang="css">
#app {
    font-family: Helvetica, Arial, sans-serif;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
