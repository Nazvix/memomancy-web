<script lang="ts" setup>

const colorMode = useColorMode()
// const isDark = computed({
//   get() {
//     return colorMode.value === 'dark'
//   },
//   set() {
//     colorMode.preference = colorMode.value === 'dark' ? 'light' : 'dark'
//   },
// })
</script>

<template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtWelcome />
    <p class="bg-red-500 dark:bg-white dark:text-amber-400">Test</p>
    <NuxtLink to="/api/login" external>
      Sign in
    </NuxtLink>
    <NuxtLink to="/api/register" external>
      Sign up
    </NuxtLink>
  </div>
</template>