<template>
  <div class="h-screen flex items-center justify-center">
    <div>
      Hello: {{ ping.hello }}
    </div>
  </div>
</template>

<script lang="ts" setup>
const response = await fetch('http://localhost:8000/ping')
const ping = await response.json()
</script>
