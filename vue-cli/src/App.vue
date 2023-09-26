<!-- template 하위에는 하나의 element만 있어야한다.-->
<template>
  <div>
    <app-header v-bind:propsdata="str" v-on:renew="renewStr"></app-header>
    {{ msg }}
  </div>

</template>

<script>
  import AppHeader from './components/AppHeader.vue';
  export default {
    data(){
      return {
        msg : 'hi',
        str : '으랏차차차차!!'
      }
    },
    components:{
      'app-header':AppHeader
    },
    methods:{
      renewStr(){
        this.str = '데이터 바뀜';
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>