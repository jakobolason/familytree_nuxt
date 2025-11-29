<script setup lang="ts">
  const { signIn } = useAuth()
  const credentials = { email: 'admin@admin', password: "admin"}
</script>
<template>
  <div>
    <p> Log in here </p>
    <UButton @click="signIn(credentials, {callbackUrl: '/'})"> here </UButton>
  </div>
</template>
