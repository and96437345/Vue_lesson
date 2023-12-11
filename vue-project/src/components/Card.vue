<script setup>
export default {
  data() {
    return {
      count: 0
    }
  },
  methods: {
    inc() {
      this.count++
    }
  }
}
import { Ref } from 'vue'
let count = ref(0)
function inc() {
  count.value++
}

defineProps({
  title: String,
  price: Number,
  isAdded: Boolean
})
</script>

<template>
  <div class="card">
    <svg>
      <use></use>
    </svg>
    <div class="card__title">{{ title }}</div>
    <div class="card__price">{{ price }}</div>
    <!-- <h2>{{ count }}</h2>
    <button @click="inc()">Добавить 1</button>
    <input v-modal="count" /> -->
  </div>
</template>

<style></style>
