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
          <div class="content-item">
            <h2 class="content-item-title">哪里能找到各行业的分析研究报告？</h2>
            <div class="content-item-describe">
              <p>Ethan： 刚入职不久，组里的尼泊尔大哥离职了，我接了他的活。第一天就被三万行的文件震惊了，一个文件里有几十个class，命名不规范，缩进随心所欲，…<span>阅读全文 <i class="el-icon-arrow-down"></i></span></p>

            </div>
            <div class="content-item-operation">
              <p class="zan-style"><i class="el-icon-caret-top"></i> 赞同 8888</p>
              <p class="zan-style"><i class="el-icon-caret-bottom"></i></p>
              <p class="operation"><i class="iconfont icon-comment"></i> 8888 条评论</p>
              <p class="operation"><i class="iconfont icon-share"></i> 分享</p>
              <p class="operation"><i class="el-icon-star-on"></i> 收藏</p>
              <p class="operation"><i class="iconfont icon-luck"></i> 喜欢</p>
              <p class="operation">...</p>
            </div>
            <div class="content-item-comment">
              <div class="comment-nav">
                <p>633 条评论</p>
                <p><i class="el-icon-sort reverse-90"></i> 切换为时间排序</p>
              </div>
              <p class="comment-chiosness">精选评论（12）</p>
              <div class="comment-detail">
                <div class="detail-head">
                  <div class="detail-head-left">
                    <img @mouseenter="mouseenterHeadimg" @mouseleave="mouseleaveHeadimg" src="../assets/image/v2-04086f9d7f89a820647674faffcbc313_im.jpg">
                    <p>倍率</p>
                  </div>
                  <p>24 天前</p>
                </div>
                <div class="detail-infomation">
                  <p class="detail-info">哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈哈</p>
                  <div class="detail-operation">
                    <p><i class="iconfont icon-zan"></i> 887</p>
                    <p><i class="iconfont icon-dafu"></i> 查看回复</p>
                    <p><i class="iconfont icon-huifu"></i> 回复</p>
                    <p><i class="iconfont icon-zan reverse-180"></i> 踩</p>
                    <p><i class="iconfont icon-qizhi"></i> 举报</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <AsideComponent></AsideComponent>
    </div>
  </div>
</template>

<script>
  import AsideComponent from "./Aside.vue";
  export default {
    name: 'Index',
    data () {
      return {

      }
    },
    methods:{
      mouseenterHeadimg(){
        console.log(this);
        console.log(123);
      },
      mouseleaveHeadimg(){
        console.log(123);
      },
    },
    components:{
      AsideComponent,
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
  .content-item{
    padding: 20px 20px;
    display: flex;
    flex-direction: column;
  }
  .content-item-title{
    font-size: 18px;
    font-weight: 600;
  }
  .content-item-describe{
    margin-top: 10px;
    word-break: break-word;
    line-height: 1.6;
    display: flex;
  }
  .content-item-operation{
    display: flex;
    align-items: center;
    padding: 10px 0px;
    color: #646464;
    background: #fff;
    line-height: 30px;
  }
  .zan-style{
    color: #0084ff;
    background: rgba(0,132,255,.1);
    border-color: transparent;
    padding: 0 12px;
    border-radius: 3px;
    margin-right: 5px;
  }
  .operation{
    color: #8590a6;
    margin-left: 24px;
  }
  .content-item-describe span{
    padding: 0;
    margin-left: 4px;
    color: #175199;
  }
  .content-item-comment{
    border: 1px solid #ebebeb;
    box-shadow: 0 1px 3px rgba(26,26,26,.1);
    background: #fff;
    margin-top: 12px;
    border-radius: 4px;
  }
  .comment-nav{
    height: 50px;
    display: flex;
    justify-content: space-between;
    line-height: 50px;
    padding: 0 20px;
  }
  .comment-nav p:first-child{
    font-size: 15px;
    font-weight: 600;
    color: #1a1a1a;
  }
  .comment-nav p:last-child{
    color: #8590a6;
    font-size: 14px;
  }
  .comment-chiosness{
    padding: 10px 20px;
    font-size: 14px;
    color: grey;
    background-color: #f6f6f6;
    font-weight: 600;
  }
  .reverse-90{
    transform: rotate(90deg);
  }
  .reverse-180{
    display: inline-block;
    transform: rotate(180deg);
  }
  .detail-head{
    position: relative;
    height: 24px;
    padding-right: 3px;
    padding-left: 1px;
    margin-bottom: 4px;
    line-height: 24px;
    display: flex;
    justify-content: space-between;
  }
  .detail-head img{
    height: 100%;
    margin-right: 8px;
  }
  .detail-head-left{
    display: flex;
    line-height: 24px;
  }
  .comment-detail{
    position: relative;
    flex-shrink: 0;
    padding: 12px 20px 10px;
    font-size: 15px;
  }
  .detail-infomation{
    padding-left: 33px;
    line-height: 24px;
  }
  .detail-operation{
    display: flex;
  }
  .detail-operation p{
    line-height: 24px;
    margin-right: 20px;
    color: #8590a6;
  }
</style>
