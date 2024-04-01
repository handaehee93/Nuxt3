<!-- [...파라미터 이름].vue 를 통해 설정되지 않은 라우팅 경로로 요청이 들어왔을 경우 
해당 요청을 받는 페이지를 만들 수 있다. -->
<template>
  <div>
    {{ $route.params.slug }}
  </div>
</template>

<script setup lang="ts"></script>

<style scoped></style>
