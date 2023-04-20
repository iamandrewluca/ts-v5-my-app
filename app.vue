<template>
  <div>
    {{ firstItem }}
  </div>
</template>

<script setup lang="ts">
interface Query {
  contents?: {
    data: string[]
  }
}

let query: Query | undefined = {}
let firstItem = query?.contents?.data.at(0)
</script>
