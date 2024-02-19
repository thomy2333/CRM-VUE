<script setup>
    import { RouterLink } from 'vue-router';

    defineProps({
        to: {
            type: String
        }
    })
</script>

<template>
    <RouterLink 
        :to="{ name: to }"
        class="block md:inline-block rounded bg-blue-800 py-2 px-3 text-white uppercase font-bold text-sm shadow hover:bg-blue-600"
    >
        <slot></slot>
    </RouterLink>
</template>