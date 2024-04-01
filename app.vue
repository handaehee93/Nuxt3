<template>
  <q-layout view="hHh lpR fFf">
    <q-header elevated class="bg-dark text-white">
      <q-toolbar>
        <q-toolbar-title>Vue Master Course</q-toolbar-title>
        <q-btn stretch flat label="Home 페이지로 이동" to="/" />
        <q-separator dark vertical />
        <q-btn stretch flat label="About 페이지로 이동" to="/about" />
      </q-toolbar>
    </q-header>
    <q-page-container :style="pageContainerStyle">
      <!-- NuxtPage라는 특수 컴포넌트를 사용하면 해당 부분에 url에 매핑되는 page 컴포넌트가 렌더링 된다. -->
      <NuxtPage />
    </q-page-container>
  </q-layout>
</template>
<script setup lang="ts">
// computed라는 것도 vue에서 제공하는 api인데 별다른 import 없이 사용할 수 있다.
const pageContainerStyle = computed(() => ({
  maxWidth: '1080px',
  margin: '0 auto',
}));
</script>
