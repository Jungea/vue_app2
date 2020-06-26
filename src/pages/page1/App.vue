<template>
  <div id="app">
    <h1>페이지1</h1>
    <Counter1 title="카운터1" description="첫째 컴포넌트" />
    <Counter1 title="카운터1" description="첫째 컴포넌트" />
  </div>
</template>

<script>
import Counter1 from './Counter1.vue'

export default {
  name: 'App',
  components : { Counter1 }
}
</script>