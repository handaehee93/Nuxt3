<!-- 동적 파라미터를 받는 경로를 폴더로 만들고, 그 아래 [ 파라미터 key 값 ].vue를 만들면 동적 파라미터를 받는 페이지를 만들 수 있다. -->
<!-- 아래의 파일은 course 경로 아래 id라는 이름으로 파라미터를 가져오는 [id].vue 파일이기 때문에 $route.params로 파라미터를 출력하면
{"id" : "전달한 파라미터"} 형식으로 파라미터를 가져오는 것을 확인할 수 있을 것이다.-->
<template>
  <q-page padding>
    <h2>Course</h2>
    <div>
      {{ $route.params }}
    </div>
  </q-page>
</template>

<script setup lang="ts">
// useRoute를 통해서도 파라미터를 가져올 수 있다.
const route = useRoute();
console.log('파리미터 출력', route.params.id);
</script>

<style scoped></style>
