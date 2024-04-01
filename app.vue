<template>
  <!-- NuxtLayout 이라는 컴포넌트를 사용해서 layouts 폴더 아래 레이아웃 파일을 불러오고, 레이아웃 파일의 slot 부분에 아래 NuxtPage를 렌더링 -->
  <!-- 만약 아래에서 <NuxtPage>가 아니라 <div> hello </div>로 바꾸면 slot 부분에 해당 태그가 렌더링 되는 것. -->
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>
<script setup lang="ts"></script>
