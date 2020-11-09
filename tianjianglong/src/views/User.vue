<template>
    <div class="User">
    <div class="pcbar">
        
<div class="pcbar__bd w1200">
    <a href="#" class="pcbar__bd__logo">
        <img src="//img.alicdn.com/tfs/TB19yBbRSzqK1RjSZFLXXcn2XXa-230-104.png" alt="" >
    </a>
    <a href="#" class="pcbar__bd__btn">
     English
    </a>
</div>
    </div>
        <div class="ui-min">
       <img src="../assets/15.png" alt="" class="ui-img">
      <div class="ui-div">
          <h2>登录</h2>
用户名:<input type="text" v-model="xx" ><br><br>
    密码:<input type="password"  v-model="yy"><br>
      <button @click="ye" style="height:30px;width:80px;background-color:red; margin: 10px auto;">登录</button>
    
      <button @click="min" style="height:30px;width:80px;background-color:red; margin: 10px 20px;">注册</button>
          <!-- <input type="text" v-model="xx">
        <input type="text" v-model="yy">
        <button @click="dianji">注册</button> -->
      </div>
      </div>

 <div >
     <ul class="dem-item">
       <li class="dem-item_list" >
         <a href="#">帮助中心</a>
       </li>
       <li class="dem-item_grep">|</li>
       <li class="dem-item_list">
         <a href="#">公司介绍</a>
       </li>
        <li class="dem-item_grep">|</li>
       <li class="dem-item_list">
         <a href="#">品牌识别</a>
       </li>
       <li class="dem-item_grep">|</li>
       <li class="dem-item_list">
         <a href="#">公司大事记</a>
       </li>
       <li class="dem-item_grep">|</li>
       <li class="dem-item_list">
         <a href="#">协议及隐私权政策</a>
       </li>
       <li class="dem-item_grep">|</li>
       <li class="dem-item_list">
         <a href="#">廉正举报</a>
       </li>
       <li class="dem-item_grep">|</li>
       <li class="dem-item_list">
         <a href="#">联系合作</a>
       </li>
       <li class="dem-item_grep">|</li>
       <li class="dem-item_list">
         <a href="#">招聘信息</a>
       </li>
       <li class="dem-item_grep">|</li>
       <li class="dem-item_list">
         <a href="#">防骗秘籍</a>
       </li>
     </ul>
   </div>
   <br/>
   <br/>
   
     <div class="footer__ft" >
       <div class="footer__ft_fl">
         <a href="#" class="footer__ft__logo">
           <img src="https://img.alicdn.com/tfs/TB1otMASmzqK1RjSZPxXXc4tVXa-167-60.png" alt="">
          
         </a>
         <div class="footer__ft__code__box">
           <img class="footer__ft__code" src="//img.alicdn.com/tfs/TB1TBEJSkvoK1RjSZFNXXcxMVXa-280-280.jpg" alt="">
            <span>App下载</span>
         </div>
       </div>
      <div class="footer__ft_fr">
      <div class="footer__fr__contact">
        <a href="#" class="footer__fr__contact__btn alime">在线客服</a>
        
      </div>
      <br/>
      <br/>
     
      <ul class="footer__ft__words">
        <li class="footer__ft__certificate">
          <a href="#">京ICP证031057号</a>
        </li>
        <li class="footer__ft__grep">|</li>

        <li class="footer__ft__certificate">
          <a href="#">京ICP备11043884号</a>
        </li>
        <li class="footer__ft__grep">|</li>
        <li class="footer__ft__certificate">
          <a href="#">京公网安备11010502037341号</a>
        </li>
        <li class="footer__ft__grep">|</li>
         <li class="footer__ft__certificate">
          <a href="#">广播电视节目制作经营许可证(京)字第02253号</a>
        </li>
      
      </ul>
      <ul class="footer__ft__words">
        <li class="footer__ft__certificate">
          <a href="#">网络文化经营许可证 京网文[2019]4082-420号</a>
        </li>
        <li class="footer__ft__grep">|</li>

        <li class="footer__ft__certificate">
          <a href="#">营业性演出许可证京市演587号</a>
        </li>
       
          </ul>
        <ul class="footer__ft__words">
           <li class="footer__ft__certificate">
           网络文化经营许可证 京网文[2019]4082-420号
        </li>
          <li class="footer__ft__certificate">
          <a href="#">大麦网</a>
        </li>
        <li>Copyright 2003-2020 All Rights Reserved</li>
          
        </ul>
        <ul class="footer__ft__words">
           <li class="footer__ft__certificate">
             举报投诉：damai_tousu@member.alibaba.com   浙江省杭州市余杭区文一西路969号
           </li>
        </ul>
          <ul class="footer__ft__words">
           <li class="footer__ft__certificate">
           违法不良信息举报电话：020-62108294
           </li>
        </ul>
<div class="footer__ft__img">
     <a href="#">
    <img src="//img.alicdn.com/tfs/TB1gw_ZxNWYBuNjy1zkXXXGGpXa-131-32.gif" alt="">
  </a>
  <a href="#">
    <img src="//img.alicdn.com/tfs/TB1ZO80pyOYBuNjSsD4XXbSkFXa-141-41.png" alt="">
  </a>
   <a href="#">
    <img src="//img.alicdn.com/tfs/TB1Y580pyOYBuNjSsD4XXbSkFXa-83-50.png" alt="">
  </a>
    <a href="#">
    <img src="//img.alicdn.com/tfs/TB1pM_ZxNWYBuNjy1zkXXXGGpXa-114-40.png" alt="">
  </a>
   
  <a href="#">
    <img src="//img.alicdn.com/tfs/TB1C4nNxTlYBeNjSszcXXbwhFXa-114-42.png" alt="">
  </a>

  
</div>
    
     
  

      </div>

  


     </div>
    










      
    </div>
</template>
<script>
//导入qs

import  storage from '../storage.js'

export default {
    name:"User",
data(){
    return{
        xx:'',
        yy:'',
        userInfo:{
   //这里的数据保证跟数据接口一致
   userid:'',
   userpwd:'',
//    email:'',

        }
    }
},
methods:{
    ye(){
 
if ((this.xx==storage.Getstorage("用户名"))&&(this.yy==storage.Getstorage("密码"))) {
    alert("登录成功");
     this.$router.push({
         path:"/"
         });
} else {
    alert("检查你的密码和用户名");
}

} ,
min(){
     this.$router.push({
         path:"/login"
         });
}

    // dianji(){
    // storage.Setstorage("用户名",this.xx);
    //     storage.Setstorage("密码",this.yy);
        
    //     this.$router.push({
    //         path:"/login"
    //     });
    // },
//    register(){
//        this.$Axios.post(
//            "../views/login.vue",
//            qs.stringify(this.userInfo),
//            {
//                // 这里qs使用的stringify方法可以将对象序列化，形成json的形式进行数据获取
//                headers:{'content-type':'multipart/form-data'}
//         }
//        ).then(res=>{
//            console.log(res);
//            // 当获取数据的状态码等于1时，相当于获取到了
//            if (res.data.status ==1) {
//                var flag=window.confirm('确定注册吗？');
//                if (flag) {
//                    //跳转页面
//                    this.$router.replace("../views/Home.vue");
//                }
//            }
//        })
//    }
}


}
</script>
<style lang="scss">
*{
    margin: 0;
    padding: 0;
}

.munt{
    margin: 0 auto;
  
    height: 300px;
    // border: 1px solid #ebebeb;
}                   
.ui-img{
    width: 2000px;
    height: 500px;
  
}
.ui-div{
    width: 430px;
    height: 380px;
   position: relative;
   top: -480px;
   right: -1537px;
        box-sizing: border-box;
    // padding: 0;
    // margin: 0;
    border: 1px solid red;
}
.ui-min{
    width: 2000px;
    height: 500px;
    margin: 10px auto;
    border: 1px solid aqua;
}
.munt_id_btn{
    float: right;
    margin-top:100px ;
    width: 180px;
    height: 300px;
    line-height: 38px;
    overflow: hidden;
    text-align: center;
    border: 2px solid aqua;
    font-size: 20px;
    color: red;
    text-decoration: none;
}
a{
    text-decoration: none;
}
.pcbar{height:90px; border: 1px solid #ebebeb;} 
.pcbar__bd{width:1200px;margin:0 auto;height:90px} 
.pcbar__bd__logo img{float:left;*display:inline;margin-top:24px;width:108px;height:48px} 
.pcbar__bd__btn{
    float:right;*display:inline;margin-top:24px;width:121px;height:38px;line-height:38px;overflow:hidden;text-align:center;border:1px solid #ebebeb;font-size:14px;color:#888;text-decoration:none;} 
    .pcbar__bd__btn:hover{text-decoration:none}
    .dem-item{
       display: flex;
    align-items: center;
    justify-content: center;
    width: 1800px;
    margin: 10px auto;
    padding: 36px 0;
    text-align: center;
    zoom: 1;
    border: 1px solid #ebebeb;
}
.dem-item_grep{
  float: left;
  padding: 0 24px;
  font-size: 20px;
}
.dem-item_list{
  float: left;
  color: #111;
  font-size: 15px;
}
.dem-item_list a:link{
   color: #111;
}
.dem-item_list a:hover{
   color: red;
}

.footer__ft {
    padding-bottom: 58px;
    zoom: 1;
    width: 1800px;
    height: 200px;
      margin: 10px auto;
    padding: 36px 0;
    border: 1px solid #ebebeb;
}
.footer__ft_fl {
    float: left;
    margin-right: 100px;
}
.footer__ft__logo{
  
   zoom: 1;
    float: left;
    margin-top: 20px;
    } 
    .footer__ft__code__box {
    float: left;
    width: 87px;
    text-align: center;
    margin-left: 40px;
}
.footer__ft__code {
    display: block;
    width: 87px;
    height: 87px;
    margin-bottom: 8px;
}
.footer__ft_fr {
    float: left;
}
.footer__fr__contact {
    zoom: 1;
    padding-bottom: 10px;
}
.footer__fr__contact__btn {
    float: left;
    display: block;
    width: 98px;
    height: 27px;
    line-height: 27px;
    text-align: center;
    background-color: #ff1268;
    color: #fff;
    font-size: 14px;
    border-radius: 20px;
}
.footer__ft__words {
    padding-bottom: 6px;
    zoom: 1;
}
.footer__ft__words:after {
    display: block;
    clear: both;
    visibility: hidden;
    height: 0;
    overflow: hidden;
    content: '.';
}
.footer__ft__words li {
    float: left;
    font-size: 13px;
    color: #111;
}
.footer__ft__grep {
    padding: 0 15px;
}
.footer__ft__img {
  margin-left:-420px;
    padding-top: 30px;
}
li,ul{
  list-style: none;
}
</style>