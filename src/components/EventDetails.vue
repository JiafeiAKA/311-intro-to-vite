<template>
    <div class="event-card">
        <h2>{{ event.category }}</h2>
        <span>{{ event.organizer }}</span>
    </div>
  </template>
  
  <script setup lang="ts">
  import { defineProps } from 'vue'
  import { Event } from '@/type'
  
  defineProps<{ event: Event }>()
  </script>
  
  <style scoped>
.event-card {
  padding: 20px;
  width: 250px;
  cursor: pointer;
  border: 1px solid #39495c;
  margin-bottom: 10px;
  text-align: right;
}
.event-card:hover {
  transform: scale(1.01);
  box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
}
  </style>
  