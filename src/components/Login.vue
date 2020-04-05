<template>
  <div class="login">
    <div class="login-wrapper">
      <div class="login-nav">
        <p class="login-nav-active">免密登陆</p>
        <p>密码登陆</p>
      </div>
      <form :model="formLabelAlign" class="login-form">
        <div class="login-flex-wrapper login-input-item">
          <label class="label">中国 +86</label>
          <i></i>
          <div class="content">
            <input type="text" placeholder="请输入手机号">
          </div>
        </div>
        <div class="login-flex-wrapper login-input-item">
          <div class="content">
            <input type="text" placeholder="请输入验证码">
          </div>
          <label class="label">获取验证码</label>
        </div>
        <el-row style="margin-top: 24px;">
          <el-button style="width: 100%;" type="primary">注册/登陆</el-button>
        </el-row>
        <p class="login-explain">
          未注册手机验证后自动登录，注册即代表同意<a href="https://www.zhihu.com/terms">《知乎协议》</a><a href="https://www.zhihu.com/term/privacy">《隐私保护指引》</a>
        </p>
        <div class="login-flex-wrapper login-input-item">
          <label class="label label-100">社交账号登陆</label>
          <div class="content login-channel">
            <p>微信</p>
            <p>QQ</p>
            <p>微博</p>
          </div>
        </div>
      </form>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
  import Footer from './footer.vue'
  export default {
    name: 'Login',
    data () {
      return {
        labelPosition: 'left',
        formLabelAlign: {
          tel: '',
          verify: '',
        }
      }
    },
    components:{
      Footer:Footer
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .login{
    position: fixed;
    height: 100%;
    width: 100%;
    background-color: #b8e5f8;
    background-image: url(../assets/image/sign_bg.db29b0fb.png);
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    align-content: center;
    justify-content: center;
    align-items: center;
  }
  .login-wrapper{
    background-color: antiquewhite;
    width: 400px;
    height: auto;
    padding: 0 24px;
    background: #fff;
  }
  .login-nav{
    display: flex;
    height: 60px;
    line-height: 60px;
    font-size: 16px;
  }
  .login-nav p{
    margin-right: 24px;
    cursor: pointer;
  }
  .login-nav-active{
    font-weight: 600;
    border-bottom: 3px solid #0084ff;
  }
  .login-form{
    margin-top: 24px;
  }
  .login-flex-wrapper{
    display: flex;
  }
  .login-flex-wrapper .label{
    flex: 0 0 80px;
    width: 80px;
    text-align: center;
    line-height: 29px;
  }
  .login-flex-wrapper i{
    width: 1px;
    background-color: #ccc;
    margin: 0 5px;
  }
  .login-flex-wrapper .content{
    flex: 1;
    display: flex;
  }
  .content input {
    width: 100%;
    border: none;
    height: 100%;
    padding-left: 15px;
  }
  .login-input-item{
    height: 50px;
    padding: 10px 0;
    border-bottom: 1px solid #ccc;
  }
  .login-explain{
    font-size: 13px;
    padding: 12px 0;
    line-height: 17px;
    border-bottom: 1px solid #ccc;
    color: grey;
  }
  .login-explain a{
    color: gray;
  }
  .label-100{
    flex: 0 0 100px !important;
    width: 100px !important;
  }
  .login-channel{
    flex-direction: row-reverse;
  }
  .login-channel p{
    padding: 0 10px;
    line-height: 29px;
  }
</style>
