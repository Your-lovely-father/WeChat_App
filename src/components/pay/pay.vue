<template>
  <div class="pay">
        <div class="nav">
            <p @click="go()">&lt;</p>
            <p>二 维 码 收 款</p>
            <p></p>
        </div>
        <div class="image">
            <img src="../../assets/images/weixin4.png" alt="">
        </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  },
  methods: {
      go(){
          this.$router.go(-1)
      }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.pay{
    background: #e6b83e;
    position: fixed;
    top: 0;
    width: 100%;
    height:100%;
}
.nav{
    width: 100%;
    height: 80px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    color: #ffffff;
    font-size: 16px;
    font-weight: 550;
}
.nav>p:nth-child(1){
    font-size: 20px;
    padding-left: 30px;
}
.image{
    width: 96%;
    margin: 0 auto;
}
.image>img{
    width: 100%;
}
</style>
