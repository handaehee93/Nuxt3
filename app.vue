<template>
  <q-layout view="hHh lpR fFf">
    <q-header elevated class="bg-dark text-white">
      <q-toolbar>
        <q-toolbar-title>Vue Master Course</q-toolbar-title>
      </q-toolbar>
    </q-header>
    <q-page-container :style="pageContainerStyle">
      <q-page padding>
        <div class="q-my-xl text-center">
          <div class="text-h4">All Courses</div>
          <p class="q-mt-sm text-grey-8">
            웹 개발 입문부터 실전까지 학습해보세요.
          </p>
        </div>
        <div class="row q-col-gutter-lg">
          <div v-for="n in 3" :key="n" class="col-12 col-md-4 col-sm-6">
            <!-- components 디렉토리에 만든 컴포넌트 파일은 별다른 import 없이 사용할 수 있다. -->
            <CourseCard />
          </div>
        </div>
      </q-page>
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
