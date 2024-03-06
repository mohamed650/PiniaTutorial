<script setup>
import Counter from '@/components/Counter.vue';
import { storeToRefs } from 'pinia';
import { useAuthStore } from '@/stores/auth.js'

const authStore = useAuthStore();

</script>

<template>
  <main>
    <div v-if="authStore.isAuthenticated">
      User Name is: {{ authStore.fullName }}
    </div>
    
    <Counter />
  </main>
</template>
