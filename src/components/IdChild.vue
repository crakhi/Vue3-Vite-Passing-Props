<template>
  ID: {{ idP }}
  <br />
  <br />
  <br />
</template>

<script setup>
import { ref, defineProps } from 'vue'
const props = defineProps(['idP'])
</script>
