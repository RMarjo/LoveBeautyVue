<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="greetings">
    <h1>{{ msg }}</h1>
    <h3>
      M'occuper de vous n'est pas un travail. C'est une passion, un bonheur,
      une chance.
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 3rem;
  position: relative;
  top: -10px;
  color: var(--color-heading);
}

h3 {
  font-size: 1.4rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {

  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
