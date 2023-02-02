<template>
  TITLE: {{ titleP }}
  <br />
  <br />
  <br />
</template>

<script setup>
import { ref, defineProps } from 'vue'
const props = defineProps(['titleP'])
</script>
