<script setup>
import { ref } from "vue";

const contacts = ref([
  { name: "John Doe", phone: "123-456-7890" },
  { name: "Jane Smith", phone: "987-654-3210" },
]);
</script>

<template>
  <div>
    <h2>Saved Contacts</h2>
    <ul>
      <li v-for="contact in contacts" :key="contact.phone">
        {{ contact.name }} - {{ contact.phone }}
      </li>
    </ul>
  </div>
</template>
