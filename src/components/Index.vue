<template>
  <div id="index">
    <div class="main-wrapper">
      <div class="content-wrapper">
        <a class="content-poster">
          <img src="../assets/image/poster.jpg">
        </a>
        <div class="content-list">
          <div class="content-nav">
            <p class="active">推荐</p>
            <p>关注</p>
            <p>热榜</p>
          </div>
        </div>
      </div>
      <div></div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Index',
    data () {
      return {

      }
    }
  }
</script>

<style scoped="">
  .main-wrapper{
    display: flex;
    width: 1032px;
    padding: 0 16px;
    margin: 10px auto;
  }
  .content-wrapper{
    width: 694px;
    margin-right: 10px;
  }
  .content-poster img{
    width: 100%;
    margin-bottom: 10px;
  }
  .content-list{
    box-shadow: 0 1px 3px rgba(26,26,26,.1);
    background: #fff;
  }
  .content-nav{
    display: flex;
    border-bottom: 1px solid #f0f2f7;
    height: 60px;
    line-height: 60px;
    padding: ;
  }
  .content-nav p{
    font-size: 16px;
    margin: 0 22px;
  }
  .content-nav .active{
    color: #0084ff;
    font-weight: 500;
  }
</style>
