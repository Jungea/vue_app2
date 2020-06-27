<template>
  <div id="app">
    <h1>페이지4</h1>
    <button type="button" @click="save"><font-awesome-icon icon="check" /> 저장</button>
    <button type="button" @click="cancel"><font-awesome-icon icon="ban" /> 취소</button>
    <button type="button" @click="remove"><font-awesome-icon icon="trash-alt" /> 삭제</button>
    <hr />
    <MyButton1 text="저장" @click="save" />
    <MyButton2 text="취소" icon="ban" @click="cancel" />
    <MyButton3 icon="trash" @click="remove">삭제</MyButton3>
  </div>
</template>

<script>
import MyButton1 from "./MyButton1.vue"
import MyButton2 from "./MyButton2.vue"
import MyButton3 from "./MyButton3.vue"

export default {
  name: 'App',
  methods: {
    save() {
      alert("저장 클릭");
    },
    cancel() {
      alert("취소 클릭");
    },
    remove() {
      alert("삭제 클릭");
    },
  },
  components: { MyButton1, MyButton2, MyButton3 }
}
</script>

<style scoped>
div#app { padding: 0 30px 30px 30px; margin: 30px auto; max-width: 400px;
      border: 1px solid #ccc; box-shadow: 3px 3px 3px #aaa; }
button { padding: 0.4em 1.5em; margin-right: 4px; }
</style>