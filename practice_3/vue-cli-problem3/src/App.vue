<template>
  <div id="app">
    
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {
    
  },
  data() {
    return {
      movieList: [
        {
          name: '블랙 팬서-와칸다 포에버', desc: `“와칸다를 지켜라!”
      거대한 두 세계의 충돌, 운명을 건 최후의 전투가 시작된다!`
        },
        { name: '[2022 LOL] 월드챔피언십 결승', desc: '[2022 LoL] 월드챔피업십 결승전 ' },
        { name: '자백', desc: '불륜 사실을 폭로하겠다는 협박을 받고 향한 호텔에서 의문의 습격을 당한 유민호(소지섭).' },
        { name: '고속도로 가족', desc: '고속도로 휴게소에서 텐트를 집, 밤하늘의 달을 조명 삼아 살고 있는 기우(정일우)와 가족들. ' },
        { name: '리멤버 ', desc: '뇌종양 말기, 80대 알츠하이머 환자인 한필주. 일제강점기 때 친일파들에게 가족을 모두 잃었다.' },
      ]
    }
  }
}
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
