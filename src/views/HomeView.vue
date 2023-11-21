<script setup lang="ts">
import dades from "@/data.json";
import DestinationShow from "@/views/DestinationShow.vue";
</script>

<template>
    <div>
        <RouterLink
            v-for="destination in info"
            :key="destination.id"
            :to="{ name: 'destination.show', params: { id: destination.id } }"
        ></RouterLink>
        <h2>{{ destination.name }}</h2>
        S
    </div>
</template>
