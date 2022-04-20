<template>
  <div>
    <div>
      Hello: {{ ping.hello }}
    </div>
  </div>
</template>

<script lang="ts" setup>
const response = await fetch('http://localhost:8000/ping')
const ping = await response.json()
</script>
