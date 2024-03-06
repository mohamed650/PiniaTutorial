<template>
    <div>
        <br>
        <button @click="store.increment">+</button>
        Count Value: {{ store.count }}
        <button @click="store.decrement">-</button>
        <br>
        Counter moved to {{ store.countDigitLength }} digit length
    </div>
</template>

<script setup>
import { useCounterStore } from '@/stores/counter';
const store = useCounterStore();

</script>