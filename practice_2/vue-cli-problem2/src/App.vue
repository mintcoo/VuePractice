<template>
  <div id="app">
    <button @click="clickBtn">PageA</button>
    <button @click="clickBtn">PageB</button>
    <p><input v-model="testData" type="text" placeholder="A페이지 보낼 데이터 입력"></p>
    <PageA v-if="checkPage('PageA')" :go-data="testData"/>
    <PageB v-if="checkPage('PageB')"/>
  </div>
</template>

<script>
import PageA from '@/components/PageA';
import PageB from '@/components/PageB';

export default {
  name: 'App',
  components: {
    PageA,
    PageB,
  },
  data() {
    return {
      page: null,
      testData: null,
    }
  },
  methods: {
    clickBtn(event) {
      this.page = event.target.innerText
    },
    checkPage(pageCheck) {
      console.log('@@@',pageCheck);
      if(this.page === pageCheck) {
        return true;
      } else {
        return false;
      }
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
