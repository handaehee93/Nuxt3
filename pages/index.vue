<!-- pages 디렉토리 안에 index.vue 파일을 만들면 해당 컴포넌트가 루트 경로로 접근 했을 때 렌더링 되는 컴포넌트가 된다. -->
<template>
  <q-page padding>
    <div class="q-my-xl text-center">
      <div class="text-h4">All Courses</div>
      <p class="q-mt-sm text-grey-8">웹 개발 입문부터 실전까지 학습해보세요.</p>
    </div>
    <div class="row q-col-gutter-lg">
      <div v-for="n in 3" :key="n" class="col-12 col-md-4 col-sm-6">
        <!-- components 디렉토리에 만든 컴포넌트 파일은 별다른 import 없이 사용할 수 있다. -->
        <CourseCard />
      </div>
    </div>
  </q-page>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped></style>
