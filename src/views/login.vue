<template>
    <div id="login">
        <div class="mid">
            <img src="../assets/imgs/logo.png" alt="">
            <div>
                <i class="iconfont icon-yonghu"></i>
                <input placeholder="请输入用户名"  >
            </div>
            <div>
                <i class="iconfont icon-mima"></i>
                <input placeholder="请输入用户密码"  >
                <span class="iconfont icon-yanjing1"></span>
            </div>
            <x-button type="warn" link="/home">登录</x-button>

        </div>
    </div>
</template>
<script>
import { XInput } from 'vux'
import { XButton } from 'vux'

export default {
  components: {
    XInput,
    XButton
  }
}
</script>
<style lang="less" scoped>
@import url(../assets/css/iconfont.css);
    #login{
        >.mid{
            padding: 0 50px;
            padding-top: 30%;
            text-align: center;
            >img{
                width: 180px;
                margin-bottom: 70px;
            }
            >div{
                border-bottom: 1px solid #e6e6e6 ;
                position: relative;
                >i{
                    position: absolute;
                    left: 0;
                    top: 50%;
                    transform: translate(0,-50%);
                }
                >span{
                    position: absolute;
                    right: 0;
                    top: 50%;
                    transform: translate(0,-50%);
                    font-size: 14px;
                    color: #b3b3b3;
                }
                input{
                    outline:none;
                    background-color: transparent;
                    border: 0;
                    height: 40px;
                    width: 100%;
                    padding-left: 30px;
                }
                >input::-webkit-input-placeholder {
                    color: #cccccc;
                    font-size: 12px;
                }
                
            }
            .weui-btn{
                margin-top: 70px;
                border-radius: 22px;
                background-image: linear-gradient(90deg, 
                    #ff6f51 0%, 
                    #ff3652 100%), 
                linear-gradient(
                    #000000, 
                    #000000);
                background-blend-mode: normal, 
                    normal;
                box-shadow: 0px 10px 20px 0px 
                rgba(255, 69, 82, 0.3);
            }
        }
    }
</style>

