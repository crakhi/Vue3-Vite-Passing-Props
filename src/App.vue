<script setup lang="ts">
import { ref, mounted } from 'vue'
import IdChild from '@/components/IdChild.vue'
import BodyChild from '@/components/BodyChild.vue'
import TitleChild from '@/components/TitleChild.vue'
import axios from 'axios'

mounted () {
    axios
      .get('https://jsonplaceholder.typicode.com/posts/2')
      .then(response => (this.post = response))
  }

const post = ref({
  userId: 1,
  id: 2,
  title: 'tit',
  body: 'body',
})
</script>

<template>
  <IdChild :idP="post.id" />
  <TitleChild :titleP="post.title" />
  <BodyChild :bodyP="post.body" />
</template>
