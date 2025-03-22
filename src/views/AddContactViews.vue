<script setup>
import { ref } from "vue";

const name = ref("");
const phone = ref("");

const addContact = () => {
  if (name.value && phone.value) {
    alert(`Added: ${name.value} - ${phone.value}`);
    name.value = "";
    phone.value = "";
  } else {
    alert("Please enter valid details");
  }
};
</script>

<template>
  <div>
    <h2>Add a Contact</h2>
    <form @submit.prevent="addContact">
      <input v-model="name" placeholder="Enter Name" />
      <input v-model="phone" placeholder="Enter Phone" />
      <button type="submit">Save Contact</button>
    </form>
  </div>
</template>
