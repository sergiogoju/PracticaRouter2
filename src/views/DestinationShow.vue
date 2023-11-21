<script>
import dades from "@/data.json";
import { ref } from "vue";
import { useRoute } from "vue-router";
const info = ref(dades);

const route = useRoute()
const locationId = <number><any>route.params.id
console.log(location.id)
</script>

<template>
    <main>
        <h1>{{ info.destinations[location - 1].name }}</h1>
        <p>{{ info.destinations[location - 1].description }}</p>
        <img
            :src="'/src/assets/images/${info.destinations[location - 1].image}'"
        />
        <section id="top-experience"></section>
    </main>
</template>
