<script setup lang="ts">
    export interface contact {
        firstName: string,
        lastName: string,
        age: number
    }

    const contacts: contact[] = [
        {
            firstName: "Ivan",
            lastName: "Ivanov",
            age: 23
        },
        {
            firstName: "Petr",
            lastName: "Petrov",
            age: 25
        },
        {
            firstName: "Sidor",
            lastName: "Sidorov",
            age: 26
        },
    ];

</script>

<template>
  <div>
    <ul>
      <li v-for="contact in contacts">
        {{ contact.firstName }} {{ contact.lastName }}
      </li>
    </ul>
  </div>
</template>

<style scoped>

</style>
