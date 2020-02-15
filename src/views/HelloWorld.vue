<template>
  <div class="hello">
    <img src="../assets/img/logo.png"/>
    <div class="percentWrap">
      <percent :percent="percent" :text-name="textName" :them="theme"/>
    </div>
  </div>
</template>

<script>
// import percent from './percent'
export default {
  name: 'HelloWorld',
  // components: {percent},
  data () {
    return {
      percent: 50,
      theme: 'blueDark',
      textName: '市场占有率1'
    }
  },
  mounted() {
    setTimeout(() => {
      this.percent = 88.57
    }, 4000)
    setTimeout(()=>{
      this.textName= '市场占有率3333'
    }, 9000)
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.percentWrap {
  height: 400px;
  background-color: #42b983;
}
</style>
