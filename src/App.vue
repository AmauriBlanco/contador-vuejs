<script setup>
import { ref } from "vue";

const count = ref(0);
</script>
<template>
    <main>
        <article>
            <h1>A contagem atual é...</h1>
            <p>{{ count }}</p>
            <button @click="count--">-</button>
            <button @click="count++">+</button>
        </article>
    </main>
</template>
<style scoped>
html,
body {
    margin: 0;
    padding: 0;
    background-color: rgb(57, 212, 127);
}

main {
    min-height: 100vh;
    min-width: 100vw;
    display: grid;
    place-items: center;
    background-color: rgb(57, 212, 127);
    color: #000;
}

article {
    text-align: center;
}

h1 {
    font-weight: 400;
}

p {
    font-size: 2rem;
    font-weight: 900;
}
</style>
