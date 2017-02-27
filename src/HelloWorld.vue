<template>
<div class="hello">
    <h1 v-if="name">{{greeting}} {{name}}!!</h1>
    <h1 v-else>{{greeting}} World!!</h1>
</div>
</template>

<script>
export default {
    name: 'HelloWorld',
    props: ['name'],
    data() {
        return {
            greeting: "Hello"
        }
    }
}
</script>

<style scoped>
.hello {
    color: white;
    background-color: blue;
}
</style>
