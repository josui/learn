<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

</script>

<template>
  <div class="content">
    <h1>{{ msg }}</h1>
    <input type="text">
    <div class="float-footer">
      Float Area
    </div>
  </div>
  <div class="keyboard-area"></div>
</template>

<style scoped>
.float-footer {
  background-color: #5599dd;
  color: white;
  height: 4rem;
  width: 100%;
  position: fixed;
  bottom: 0;
}

/* .test {
  --size: 4rem;
  position: fixed;
  right: min(1rem, 100vw - env(keyboard-inset-width, 0rem));
  bottom: max(1rem, env(keyboard-inset-height, 0rem));
  width: max(var(--size), env(keyboard-inset-width, 0rem));
  height: var(--size);
  z-index: 1;
  background-color: #3f51b5;
  border-radius: min(0px, max(50px, env(keyboard-inset-width, 0rem)));
  border-radius: max(0px, min(50px, 100% - env(keyboard-inset-width)));
  box-shadow: 0 3px 10px 0 rgba(#000, 0.1);
  transition: 0.3s ease-out;
} */
</style>
