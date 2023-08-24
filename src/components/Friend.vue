<template>
  <h3>{{ name }}</h3>
  <p>
    <strong>Phone:</strong>
    {{ phone }}
  </p>
  <p>
    <strong>Email:</strong>
    {{ mail }}
  </p>
  <button @click="$emit('elimina', id)">Elimina</button>
</template>

<script>
export default {
  props: ["id", "name", "phone", "mail"],
  emits: ["elimina"],
  name: "Friend",
  return: {
    methods: {},
  },
};
</script>