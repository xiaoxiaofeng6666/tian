<template>
  <div class="home">
  <div class="dm-header-wrap">
	<div class="dm-header-box" data-spm="top">
		<a href="//www.damai.cn"><img class="i-logo" src="//img.alicdn.com/tfs/TB1fbVFfu3tHKVjSZSgXXX4QFXa-230-104.png" alt="大麦" /></a>
		<div class="location-header">
			<el-dropdown @command="handleCommand">
  <span class="el-dropdown-link">
    <img src="//img.alicdn.com/tfs/TB1XHDuxNGYBuNjy0FnXXX5lpXa-28-32.png" style="    width: 12px; 
  
    vertical-align: middle;" />下拉菜单<i class="el-icon-arrow-down el-icon--right"></i>
  </span>
 
  <el-dropdown-menu slot="dropdown">
    <el-dropdown-item command="a"  style="width:300px; padding:10px auto;">
       当前城市：  <a href="#">全国</a>
           </el-dropdown-item>
         <hr/>
    <el-dropdown-item command="b" style="margin:10px auto ;"> 当前城市：  <a href="#">
      <span>北京</span></a>
      
      <span>|</span>
      <a href="#">上海</a>
       <span>|</span>
 <a href="#">天津</a>
  <span>|</span>
  <a href="#">杭州</a>
    </el-dropdown-item>
    <el-dropdown-item command="c">热门城市：
    <a href="#">北京 </a>
    <a href="#">成都</a>
    <a href="#">深圳</a>
    <a href="#">杭州</a>
  
    </el-dropdown-item>
   
     <hr/>
       
    <el-dropdown-item command="e" divided>其他城市：
      <a href="#">深圳 </a>
    <a href="#">南京</a>
    <a href="#">西安</a>
    <a href="#">昆明</a>
    </el-dropdown-item>
  </el-dropdown-menu>
</el-dropdown>
           <!--    <span class="city-location">首页</span>
               <span class="city-location">分类</span>
			<div class="city-header-wrap">
				<div class="city-header" data-spm="city">
					<div class="now-city">
						<span class="title-city">当前城市:</span>
						<span class="name-city select-city">全国</span>
					</div>
					<div class="hot-city">
						<span class="title-city">热门城市:</span>
						<div class="list-other"></div>
					</div>
					<div class="other-city">
						<span class="title-city">其他城市:</span>
						<div class="list-other">

                        </div>
					</div>
				</div>
			</div>  -->
      
		</div>
    
		<div class="recommend-header">
			<a href="//www.damai.cn" class="type-recommend select" data-spm="dhome">首页</a>
			<a href="//search.damai.cn/search.htm?order=1" class="type-recommend" data-spm="dcategory">分类</a>
			
			
		</div>
<div class="right-header">
<div class="box-header user-header">
  <a href="#" class="J_userinfo_img">
    <img src="//img.alicdn.com/tfs/TB14UKCGQyWBuNjy0FpXXassXXa-54-54.png" class="i-box-header i-user" alt="">
  </a>
  <a href="#" class="J_userinfo_name">
   <div class="span-box-header name-user"></div>
  </a>
  <div class="login-user show">
   <el-tooltip placement="bottom">
  <div slot="content">
    <button>  <a href="/User">个人信息</a> </button>
    
    <br/>
     <button>  <a href="#">账单管理</a> </button>
      <br/>
       <button>  <a href="#">订单管理</a> </button>
        <br/>
         <button>  <a href="/login">退出登录</a> </button>
    </div>
  <el-button  ><span class="span-box-header span-user">登录</span></el-button>
</el-tooltip>
     
    <!--  -->
  </div>

  <div class="list-wrap">
    <!-- <div class="list-login">
      <a href="#" class="li-login select">个人信息</a>
      <a href="#" class="li-login">账号管理</a>
      <a href="#" class="li-login">订单管理</a>
      <a href="#" class="li-login out-login">退出登录</a>
    </div> -->
  </div>
</div>
<div class="box-header download-header">
  <img class="i-box-header i-download"  src="//img.alicdn.com/tfs/TB1A9eIGKuSBuNjy1XcXXcYjFXa-54-54.png" alt="">
    <!-- <span class="span-box-header">下载</span>
     <div class="ewm-download">
       <img class="i-ewm"   src="//img.alicdn.com/tfs/TB1TBEJSkvoK1RjSZFNXXcxMVXa-280-280.jpg" alt="">
     </div> -->
     <el-tooltip placement="top">
  <div slot="content" style="width:200px;">
    <a href="#"><img src="//img.alicdn.com/tfs/TB1TBEJSkvoK1RjSZFNXXcxMVXa-280-280.jpg" alt=""></a>
  </div>
  <el-button>下载</el-button>
</el-tooltip>
     

</div>
<div class="box-header">
  <a href="#">
    <img class="i-box-header"  src="//img.alicdn.com/tfs/TB13UKCGQyWBuNjy0FpXXassXXa-54-54.png" alt="">
  </a>
  <span class="span-box-header">English</span>
</div>

</div>
		<!-- <div class="right-header" data-spm="nick">
			<div class="box-header user-header">
				<a href="javascript:void(0)" class="J_userinfo_img" data-spm="duserinfo"><img class="i-box-header i-user" src="//img.alicdn.com/tfs/TB14UKCGQyWBuNjy0FpXXassXXa-54-54.png" /></a>
				<a href="//passport.damai.cn/accountinfo/myinfo" class="J_userinfo_name" data-spm="duserinfo">
					<div class="span-box-header name-user"></div>
				</a>
				<div class="login-user show">
					<span class="span-box-header span-user" data-spm="dlogin">登录</span>
				</div>
				<div class="list-wrap">
					<div class="list-login">
						<a href="//passport.damai.cn/accountinfo/myinfo" class="li-login select" data-spm="duserinfo">个人信息</a>
						<a href="//my.damai.cn/account/accountSafe" class="li-login" data-spm="daccountsetting">账号设置</a>
						<a href="//orders.damai.cn/orderList" class="li-login" data-spm="dordermanage">订单管理</a>
						<a href="//passport.damai.cn/account/logout" data-spm="dexit" class="li-login out-login">退出登录</a>
					</div>
				</div>
			</div>
			<div class="box-header download-header">
				<img class="i-box-header i-download" src="//img.alicdn.com/tfs/TB1A9eIGKuSBuNjy1XcXXcYjFXa-54-54.png" alt="下载" />
				<span class="span-box-header">下载</span>
				<div class="ewm-download">
					<img class="i-ewm" src="//img.alicdn.com/tfs/TB1TBEJSkvoK1RjSZFNXXcxMVXa-280-280.jpg" />
				</div>
			</div>
			<div class="box-header">
				<a href="//en.damai.cn/" data-spm="denglish">
					<img class="i-box-header" src="//img.alicdn.com/tfs/TB13UKCGQyWBuNjy0FpXXassXXa-54-54.png" alt="英文站" />
					<span class="span-box-header">English</span>
				</a>
			</div>
		</div> -->

		<div class="search-header" data-spm="searchtxt">
			<img class="i-search" src="//img.alicdn.com/tfs/TB1qv3jxGmWBuNjy1XaXXXCbXXa-34-36.png" alt="搜索" />
			<input class="input-search" placeholder="搜索明星、演出、体育赛事" data-spm="dsearchbtn" />
			<div class="btn-search" data-spm="dsearchbtn2">搜索</div>
			<div class="list-search-wrap">
				<div class="list-search">
				</div>
			</div>
		</div>
		
	</div>
  
</div>




     <!--  <div class="order-s">
        <center> 
                    <ul>
                    <li><a href="#"><img src="../assets/01.png" alt=""></a></li>
                    <li class="s1"><a href="#"><img src="//img.alicdn.com/tfs/TB1XHDuxNGYBuNjy0FnXXX5lpXa-28-32.png" alt="">全国</a>
                   
                      <ul>
                            <li><a href="#">二级菜单</a></li>
                            <li><a href="#">二级菜单</a></li>
                        </ul>
                    </li>
                    <li><a href="#"><h3>首页</h3></a></li>
                    <li><a href="#"><h3>分类</h3></a></li>
                    
                    <li class="s3">
                      
  <h3>     <el-autocomplete
  v-model="state"
  :fetch-suggestions="querySearchAsync"
  placeholder="请输入内容"
  @select="handleSelect"
></el-autocomplete></h3>

 
 
  </li>

<li class="s2">
<h3><el-button type="primary" icon="el-icon-search">搜索</el-button></h3>
</li>
  
     <li class="s4">
   
<h3>  <el-breadcrumb separator="">
  <el-breadcrumb-item><a href="/"><h3>登录/</h3></a>

  </el-breadcrumb-item>
 
  <el-breadcrumb-item><a href="/"><h3>下载/</h3></a></el-breadcrumb-item>
   <el-breadcrumb-item><a href="/"><h3>Enlish/</h3></a></el-breadcrumb-item>
    <el-breadcrumb-item><a href="/"><h3>...</h3></a></el-breadcrumb-item>
</el-breadcrumb></h3>
   
       </li>          
                   
           
                      </ul>
                    </center>      
</div>  -->
<br/>
<br/>
<br/>
<br/>
        <div class="order-head">
     
   <!-- <span class="demonstration">默认 Hover 指示器触发</span> -->
    <el-carousel height="300px">
      <el-carousel-item >
        <h3><img style="width: 1800px;, height=500px;" src="https://gw.alicdn.com/tfs/TB1QRm61lr0gK0jSZFnXXbRRXXa-1200-320.jpg" alt=""></h3>
      </el-carousel-item>
       <el-carousel-item >
        <h3><img style="width: 1800px;, height=500px;" src="https://gw.alicdn.com/tfs/TB1KiMMq7L0gK0jSZFtXXXQCXXa-1200-320.png" alt=""></h3>
      </el-carousel-item>
   <el-carousel-item >
        <h3><img style="width: 1800px;, height=500px;" src="https://gw.alicdn.com/tfs/TB1QRm61lr0gK0jSZFnXXbRRXXa-1200-320.jpg" alt=""></h3>
      </el-carousel-item>
         <el-carousel-item >
        <h3><img style="width: 1800px;, height=500px;" src="https://gw.alicdn.com/tfs/TB1KiMMq7L0gK0jSZFtXXXQCXXa-1200-320.png" alt=""></h3>
      </el-carousel-item>
    </el-carousel>
  </div>
 
    <br/>
    <br/>
        <div class="category">
          <a href="#" class="category__list">
            <span class="category__icon category__icon__ych"></span>
            <p class="category__info">演唱会</p>
          </a>
          <a href="#" class="category__list">
            <span class="category__icon category__icon__gjhj"></span>
             <p class="category__info">话剧歌剧</p>
          </a>
          <a href="#" class="category__list">
            <span class="category__icon category__icon__tyjj"></span>
             <p class="category__info">体育</p>
          </a>
          <a href="#" class="category__list">
            <span class="category__icon category__icon__qz"></span>
             <p class="category__info">儿童亲子</p>
          </a>
          <a href="#" class="category__list">
            <span class="category__icon category__icon__zlxx"></span>
             <p class="category__info">展览休闲</p>
          </a>
           <a href="#" class="category__list">
            <span class="category__icon category__icon__yyh"></span>
             <p class="category__info">音乐</p>
          </a>
           <a href="#" class="category__list">
            <span class="category__icon category__icon__xsxq"></span>
             <p class="category__info">曲苑杂坛</p>
          </a>
           <a href="#" class="category__list">
            <span class="category__icon category__icon__wdbl"></span>
             <p class="category__info">舞蹈芭蕾</p>
          </a>
            <a href="#" class="category__list">
            <span class="category__icon category__icon__dm"></span>
             <p class="category__info">二次元</p>
          </a>
           <a href="#" class="category__list">
            <span class="category__icon category__icon__lyzl"></span>
             <p class="category__info">旅游展览</p>
          </a>
        
<!-- <a href="#" class="order-item-1-1">
  <img src="../assets/02.png" alt="">
  <span class="order-item-1"></span>
  <p class="order-list">演唱会</p>
</a> -->

<!-- <a href="#" class="order-item-2-1">
  <img src="//img.alicdn.com/tfs/TB1U9R8GY9YBuNjy0FgXXcxcXXa-146-1822.png" alt="">
  <span class="order-item-2"></span>
  <p class="order-list">演唱会</p>
</a> -->


   </div>
   <div class="wanghui">
   
      <div class="icon damai">
        <el-tooltip    placement="left-start">
  <div slot="content">
   <img src="//img.alicdn.com/tfs/TB1TBEJSkvoK1RjSZFNXXcxMVXa-280-280.jpg" alt="" style="  width: 100px;
  height: 100px;">
  </div>
 <a href="#"><img src="../assets/16.png" alt="">
 <br/>
 <p>App下载</p></a>
</el-tooltip>
         <!-- <a href="#">
        <img src="" alt="">
        
         </a> -->
      </div>
      <div class=""></div>
   
</div>
    <div class="order-cun">
      
    <el-container>
      
  <el-header class="head">演唱会
    <span class="head2">查看全部</span>
  </el-header>
 
  <br/>
  <br/>
   <el-main width="500px">
 
        <img class="image" src="https://img.alicdn.com/bao/uploaded/https://img.alicdn.com/imgextra/i1/2251059038/O1CN01v47qkp2GdSGvzJciF_!!2251059038.jpg" alt="">
      <div class="box-left">
        <div class="title"><a href="#"></a>科罗娜.2020杭州草莓音乐节</div>
        <div class="details">
          "￥300起"
        </div>
        
      </div>
    <div class="min">
     <a href="#">
      <img src="../assets//03.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">2020国潮音乐嘉年华</div></a>
        <br/>
         <br/>
          <div class="min3">苏州站</div>
          <br/>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">苏州太湖园博园景区</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.11.21-11.22</div></a>
      <br/>
      <br/>
      <br/>
       <a href="#"> <span class="min5">￥488起</span></a>
      </div>

       <a href="#">
      <img src="../assets/04.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">2020王晰"歌颂" 个</div></a>
        <br/>
          <div class="min3">个巡回音乐会-------</div>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">佛山琼花大剧院</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.11.21 周六 20:00</div></a>
          <br/>
      <br/>
      <br/>
       <a href="#"> <span class="min5">￥480起</span></a>
      </div>
      
        <a href="#">
      <img src="../assets//05.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">2020嘉善大云。云上乡</div></a>
        <br/>
          <div class="min3">村音乐节</div>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">嘉兴嘉善县云澜湾温泉景区</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.11.21 周六 15:00</div></a>
           <br/>
      <br/>
      <br/>
       <a href="#"> <span class="min5">￥199起</span></a>
      </div>

    </div>
    <div class="min">
     <a href="#">
      <img src="../assets//06.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">2020谢天笑  活力岛特别场</div></a>
        <br/>
         <br/>
          <div class="min3">—【重聚】</div>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">苏州相城活力岛</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.11.21 周六 19:30</div></a>
      <br/>
      <br/>
      <br/>
       <a href="#"> <span class="min5">￥258起</span></a>
      </div>

       <a href="#">
      <img src="../assets//07.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">刘令飞 · 野路子音乐会</div></a>
        <br/>
         <br/>
          <div class="min3">北京站</div>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">糖果TANGO-雍和宫店三层</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.11.13-11.14</div></a>
          <br/>
      <br/>
      <br/>
       <a href="#"> <span class="min5">￥480起</span></a>
      </div>

        <a href="#">
      <img src="../assets//08.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">N+音乐嘉年华</div></a>
        <br/>  <br/>
          <div class="min3">苏州站</div>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">成都国际非物质文化遗产博览园</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.11.14-11.15</div></a>
           <br/>
      <br/>
      <br/>
      
       <a href="#"> <span class="min5">￥180起</span></a>
      </div>

    </div>
      </el-main>
 
 
  
</el-container>
      </div>
      <br/>
      <br/>
      <br/>
        <div class="order-cun">
      
    <el-container>
      
  <el-header class="head">体育场
    <span class="head2">查看全部</span>
  </el-header>
 
  <br/>
  <br/>
   <el-main width="500px">
 
        <img class="image" src="https://img.alicdn.com/bao/uploaded/https://img.alicdn.com/imgextra/i2/2251059038/O1CN01bANzjU2GdSGkBHEoO_!!2251059038.jpg" alt="">
      <div class="box-left">
        <div class="title"><a href="#"></a>【中甲】2020中国足球协会甲级联赛（常州赛区） </div>
       <br/>
       <br/>
       <br/>
        <div class="details">
          "￥1000起"
        </div>
        
      </div>
      <br/>
      
    <div class="min">
     <a href="#">
      <img src="../assets//09.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">2020一球致胜网球大</div></a>
        <br/>
         <br/>
          <div class="min3">奖赛</div>
          <br/>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">上海旗忠森林体育城网球中心</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.11.20-11.22</div></a>
      <br/>
      <br/>
      <br/>
       <a href="#"> <span class="min5">￥60起</span></a>
      </div>

       <a href="#">
      <img src="../assets/10.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">2020·“万科青山湖</div></a>
        <br/>
          <div class="min3">杯”南昌市首届水上...</div>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">青山湖水上运动之家-南昌赛艇运动中心</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.11.14-11.15</div></a>
          <br/>
      <br/>
      <br/>
       <a href="#"> <span class="min5">￥198起</span></a>
      </div>
      
        <a href="#">
      <img src="../assets//11.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">2020 FORMULA1 中</div></a>
        <br/>
          <div class="min3">国大奖赛（礼包&福袋...</div>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">上汽国际赛车场(上海国际赛车场)</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.07.04-2021.03.09</div></a>
           <br/>
      <br/>
      <br/>
       <a href="#"> <span class="min5">￥120起</span></a>
      </div>

    </div>
    <div class="min">
     <a href="#">
      <img src="../assets//12.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">2020 FORMULA1 中品</div></a>
        <br/>
         <br/>
          <div class="min3">国大奖赛（周边衍生...</div>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">上汽国际赛车场(上海国际赛车场)</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.03.11-12.31</div></a>
      <br/>
      <br/>
      <br/>
       <a href="#"> <span class="min5">￥35起</span></a>
      </div>

       <a href="#">
      <img src="../assets//13.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">2020 FORMULA1 中</div></a>
        <br/>
         <br/>
          <div class="min3">国大奖赛（帽品）</div>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">上汽国际赛车场(上海国际赛车场)</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.03.11-12.31</div></a>
          <br/>
      <br/>
      <br/>
       <a href="#"> <span class="min5">￥200起</span></a>
      </div>

        <a href="#">
      <img src="../assets//14.png" alt=""/></a>
      <div class="min2">
       <a href="#"> <div class="min3">2020 FORMULA1 中</div></a>
        <br/>  <br/>
          <div class="min3">国大奖赛（服装）</div>
         <br/>
            <br/>
               <br/>
        <a href="#">  <div class="min4">上汽国际赛车场(上海国际赛车场)</div></a>
        <br/>
           <br/>
              <br/>
              
      <a href="#">  <div class="min4">2020.05.19-12.31</div></a>
           <br/>
      <br/>
      <br/>
       <a href="#"> <span class="min5">￥248起</span></a>
      </div>

    </div>
      </el-main>
 
 

</el-container>
      </div>
      <br/>
      <br/>
      <br/>
      <br/>
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
    <img src="//img.alicdn.com/tfs/TB1ZO80pyOYBuNjSsD4XXbSkFXa-141-41.png" alt="">
  </a>
   <a href="#">
    <img src="//img.alicdn.com/tfs/TB1Y580pyOYBuNjSsD4XXbSkFXa-83-50.png" alt="">
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
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';
import Cank from '../views/Cank.vue';

export default {
  name: 'Home',
  data(){
    return{
      
         restaurants: [],
        state: '',
    };
    },
    // components:{
    //    Cank:require('../views/Cank.vue').default
    // },
  components:{
   "Cank":Cank
  },
    methods: {
      loadAll() {
        return [
          { "value": "三全鲜食（北新泾店）", "address": "长宁区新渔路144号" },
          { "value": "Hot honey 首尔炸鸡（仙霞路）", "address": "上海市长宁区淞虹路661号" },
          { "value": "新旺角茶餐厅", "address": "上海市普陀区真北路988号创邑金沙谷6号楼113" },
          { "value": "泷千家(天山西路店)", "address": "天山西路438号" },
          { "value": "胖仙女纸杯蛋糕（上海凌空店）", "address": "上海市长宁区金钟路968号1幢18号楼一层商铺18-101" },
          { "value": "贡茶", "address": "上海市长宁区金钟路633号" },
          { "value": "豪大大香鸡排超级奶爸", "address": "上海市嘉定区曹安公路曹安路1685号" },
          { "value": "茶芝兰（奶茶，手抓饼）", "address": "上海市普陀区同普路1435号" },
          { "value": "十二泷町", "address": "上海市北翟路1444弄81号B幢-107" },
          { "value": "星移浓缩咖啡", "address": "上海市嘉定区新郁路817号" },
          { "value": "阿姨奶茶/豪大大", "address": "嘉定区曹安路1611号" },
          { "value": "新麦甜四季甜品炸鸡", "address": "嘉定区曹安公路2383弄55号" },
          { "value": "Monica摩托主题咖啡店", "address": "嘉定区江桥镇曹安公路2409号1F，2383弄62号1F" }
      
        ];
      },
      querySearchAsync(queryString, cb) {
        var restaurants = this.restaurants;
        var results = queryString ? restaurants.filter(this.createStateFilter(queryString)) : restaurants;

        clearTimeout(this.timeout);
        this.timeout = setTimeout(() => {
          cb(results);
        }, 3000 * Math.random());
      },
      createStateFilter(queryString) {
        return (state) => {
          return (state.value.toLowerCase().indexOf(queryString.toLowerCase()) === 0);
        };
      },
      handleSelect(item) {
        console.log(item);
      }
    },
    mounted() {
      this.restaurants = this.loadAll();
    },
      handleCommand(command) {
        this.$message('click on item ' + command);
      }
  };

</script>
<style scoped lang="scss">
   @import "../css/Cank.css";
*{
  margin: 0;
  padding: 0;
}
//返回顶部
.icon .damai{
    // background-image: url(https://img.alicdn.com/tfs/TB1u1U9xmzqK1RjSZFHXXb3CpXa-64-180.png);
    //     background-position: 0 4px;
    // margin: 0 auto;
    // width: 32px;
    // height: 29px;
    // background-size: 100%;
}
.wanghui{
position: relative;
float: right;
  width: 100px;
  height: 100px;
  border: 1px solid #ebebeb
}
.dm-header-wrap{
    width: 100%;
    height: 72px;
    box-shadow: 0 2px 16px 0 rgba(220, 220, 220, 5);
}
.dm-header-box{
    width: 1200px;
    height: 100%;
    margin: 0 auto;
    position: relative;
    font-size: 0;
}
.dm-header-box .i-logo{
    width: 92px;
    height: auto;
    margin-top: 15px;
    float: left;
    margin-left: -200px;
}
//下拉框
  .el-dropdown-link {
    cursor: pointer;
    color: #409EFF;
  }
  .el-icon-arrow-down {
    
    font-size: 12px;
  }
.dm-header-box .location-header{
    display: block;
    height: 100%;
    float: left;
    position: relative;
    
    line-height: 72px;
    white-space: nowrap;
    cursor: pointer;
}
.dm-header-box  .location-header  .i-icon-location{
   width: 16px;
   display: inline-block;
   vertical-align: middle;
}
.dm-header-box .location-header .city-location{
     max-width: 60px;
     font-size: 20px;
     color: #2d2d2d;
     display: inline-block;
     vertical-align: middle;
     margin-left: 5px;
     margin-right: 5px;
     white-space: nowrap;
     overflow: hidden;
     text-overflow: ellipsis;
}
.dm-header-box .location-header .i-arrow-location{
     width: 9px;
     display: inline-block;
     vertical-align: middle;
}
.dm-header-box .location-header .city-header{
    width: 626px;
    height: 200px;
    z-index: 999;
    position: relative;
    left: -115px;
    top: 0;
    margin-top: 60px;
    background: #fff;
    border: 1px solid #f4f4f4;
    box-shadow: 0 2px 8px 0 rgba(0, 0,0, .05);
    border-radius: 2px;
    padding: 21px;
}
.dm-header-box .location-header .now-city{
   line-height: 25px;
}
.dm-header-box .location-header .title-city{
   width: 86px;
   float: left;
   display: inline-block;
   margin-right: 15px;
   vertical-align: top;
   font-size: 16px;
   color: #111;
   letter-spacing: .56px;
  
}
.dm-header-box .location-header .city-header .now-city .select-city {
    color: red;
    background-color: #ededed;
    padding: 0 10px;
    display: inline-block;
    margin-right: 15px;
    vertical-align: top;
    font-size: 16px;
    line-height: 25px;
    white-space: nowrap;
    cursor: pointer;

    letter-spacing: .56px;
    float: left;
}
.dm-header-box .location-header .city-header .hot-city {
   line-height: 25px;
   margin-top: 40px;
}
.dm-header-box .location-header .city-header .title-city{
    width: 86px;
}

    .dm-header-box .location-header .city-header .list-other {
        width: 525px;
        display: inline-block;
        line-height: 29px;
        margin-top: -3px;
    }

.dm-header-box .location-header .city-header .name-city{
    display:flex;
    justify-content: space-between;
    margin-right: 15px;
    vertical-align: top;
    font-size: 16px;
    color: #111;
    letter-spacing: .56px;
    float: left;
    line-height: 29px;
}
.dm-header-box .location-header .city-header .other-city{
    line-height: 25px;
    padding-top:15px ;
    border-top: 1px solid #ededed;
    margin-top: 15px;
    margin-right: -500px ; 
}
.dm-header-box .recommend-header{
    max-width: 220px;
    height: 100%;
    float: left;
    margin-right: -20px;
    margin-left: 40px;
    line-height: 72px;
    overflow: hidden;
}
.dm-header-box .recommend-header .select {
    color: #FF1268;
}
.dm-header-box .recommend-header .type-recommend {
    display: inline-block;
    font-size: 16px;
    color: #000;
    margin-right: 18px;
    overflow: hidden;
}
.dm-header-box a{
    cursor: pointer;
}
.dm-header-box .right-header {
    min-width: 55px;
    height: 100%;
    position: relative;
    float: right;
    line-height: 72px;
}
.dm-header-box .right-header .box-header {
    height: 100%;
    display: inline-block;
    line-height: 72px;
    cursor: pointer;
    position: relative;
    margin-left: 20px;
}
.dm-header-box .right-header .user-header .i-user {
    border-radius: 13px;
}
.dm-header-box .right-header .box-header .i-box-header {
    width: 26px;
    z-index: 20000;
    display: inline-block;
    margin-right: 4px;
    vertical-align: middle;
}
.dm-header-box .right-header .user-header .name-user {
  display: block;
    max-width: 50px;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
}
.dm-header-box .right-header .user-header .show {
    display: inline-block;
}
.dm-header-box .right-header .box-header .span-box-header {
    display: inline-block;
    vertical-align: middle;
    color: #111;
    cursor: pointer;
    font-size: 16px;
}
.dm-header-box .right-header .user-header .list-wrap {
    width: 133px;
    display: none;
    position: absolute;
    left: 50%;
    margin-left: -67px;
    top: 50px;
    z-index: 999;
}
.dm-header-box .right-header .user-header .list-login {
    width: 100%;
    position: relative;
    margin-top: 10px;
    background: #FFF;
    border: 1px solid #F4F4F4;
    box-shadow: 0 2px 8px 0 rgba(0,0,0,.05);
    border-radius: 2px;
}
.dm-header-box .right-header .user-header .list-login .li-login {
    width: 100%;
    height: 50px;
    display: block;
    line-height: 50px;
    font-size: 14px;
    color: #111;
    letter-spacing: .54px;
    text-align: center;
    border-bottom: 1px solid #F2F2F2;
}
.dm-header-box .right-header .box-header {
    height: 100%;
    display: inline-block;
    line-height: 72px;
    cursor: pointer;
    position: relative;
    margin-left: 20px;
}
.dm-header-box .right-header .box-header .i-box-header {
    width: 26px;
    z-index: 20000;
    display: inline-block;
    margin-right: 4px;
    vertical-align: middle;
}
.dm-header-box .right-header .box-header .span-box-header {
    display: inline-block;
    vertical-align: middle;
    color: #111;
    cursor: pointer;
    font-size: 16px;
}
.dm-header-box .right-header .download-header .ewm-download {
    width: 80px;
    height: 80px;
    display: none;
    position: absolute;
    top: 60px;
    left: -12px;
    z-index: 999;
    background: #fff;
    padding: 5px;
    box-shadow: 1px -1px 1px #ccc;
}
.dm-header-box a {
    cursor: pointer;
}
.dm-header-box .right-header .user-header .i-user {
    width: 26px;
    z-index: 20000;
    display: inline-block;
    margin-right: 4px;
    vertical-align: middle;
}
.dm-header-box .right-header .download-header .ewm-download .i-ewm {
    width: 100%;
}
.dm-header-box .right-header .box-header {
    height: 100%;
    display: inline-block;
    line-height: 72px;
    cursor: pointer;
    position: relative;
    margin-left: 20px;
}
.dm-header-box .right-header .box-header .i-box-header {
    width: 26px;
    z-index: 20000;
    display: inline-block;
    margin-right: 4px;
    vertical-align: middle;
}
// .dm-header-box .right-header .box-header {
//     height: 100%;
//     display: inline-block;
//     line-height: 72px;
//     cursor: pointer;
//     position: relative;
//     margin-left: 20px;
// }
// .dm-header-box .right-header .box-header .i-box-header {
//     width: 26px;
//     z-index: 20000;
//     display: inline-block;
//     margin-right: 4px;
//     vertical-align: middle;
// }
// .dm-header-box .right-header .user-header .i-user {
//     border-radius: 13px;
// }
// .dm-header-box .right-header .user-header .name-user {
//     max-width: 50px;
//     overflow: hidden;
//     text-overflow: ellipsis;
//     white-space: nowrap;
// }
// .dm-header-box .right-header .user-header .show {
//     display: inline-block;
// }
// .dm-header-box .right-header .box-header .span-box-header {
//     display: inline-block;
//     vertical-align: middle;
//     color: #111;
//     cursor: pointer;
//     font-size: 16px;
// }
// .dm-header-box .right-header .user-header .list-wrap {
//     width: 133px;
//     display: none;
//     position: absolute;
//     left: 50%;
//     margin-left: -67px;
//     top: 50px;
//     z-index: 999;
// }
// .dm-header-box .right-header .user-header .list-login {
//     width: 100%;
//     position: relative;
//     margin-top: 10px;
//     background: #FFF;
//     border: 1px solid #F4F4F4;
//     box-shadow: 0 2px 8px 0 rgba(0,0,0,.05);
//     border-radius: 2px;
// }
// .dm-header-box .right-header .user-header .list-login .li-login {
//     width: 100%;
//     height: 50px;
//     display: block;
//     line-height: 50px;
//     font-size: 14px;
//     color: #111;
//     letter-spacing: .54px;
//     text-align: center;
//     border-bottom: 1px solid #F2F2F2;
// }
// .dm-header-box .right-header .user-header .list-login .li-login {
//     width: 100%;
//     height: 50px;
//     display: block;
//     line-height: 50px;
//     font-size: 14px;
//     color: #111;
//     letter-spacing: .54px;
//     text-align: center;
//     border-bottom: 1px solid #F2F2F2;
// }
// .dm-header-box .right-header .user-header .list-login .li-login {
//     width: 100%;
//     height: 50px;
//     display: block;
//     line-height: 50px;
//     font-size: 14px;
//     color: #111;
//     letter-spacing: .54px;
//     display: none;
//     text-align: center;
//     border-bottom: 1px solid #F2F2F2;
// }
// .dm-header-box .right-header .box-header .i-box-header {
//     width: 26px;
//     z-index: 20000;
//     display: inline-block;
//     margin-right: 4px;
//     vertical-align: middle;
// }
// .dm-header-box .right-header .box-header .span-box-header {
//     display: inline-block;
//     vertical-align: middle;
//     color: #111;
//     cursor: pointer;
//     font-size: 16px;
// }
// .dm-header-box .right-header .download-header .ewm-download {
//     width: 80px;
//     height: 80px;
//     display: none;
//     position: absolute;
//     top: 60px;
//     left: -12px;
//     z-index: 999;
//     background: #fff;
//     padding: 5px;
//     box-shadow: 1px -1px 1px #ccc;
// }
// .dm-header-box .right-header .download-header .ewm-download .i-ewm {
//     width: 100%;
// }
// .dm-header-box .right-header .box-header {
//     height: 100%;
//     display: inline-block;
//     line-height: 72px;
//     cursor: pointer;
//     position: relative;
//     margin-left: 20px;
// }
.dm-header-box .search-header {
    width: 401px;
    height: 46px;
    margin-top: 10px;
    margin-right: 300px;
    line-height: 46px;
    float: right;
    position: relative;
}
.dm-header-box .search-header .i-search {
    width: 17px;
    position: absolute;
    left: 22px;
    top: 15px;
    z-index: 11;
}


.dm-header-box .search-header .input-search {
    width: 253px;
    height: 44px;
    position: absolute;
    left: 0;
    top: 0;
    z-index: 10;
    font-size: 16px;
    background-color: transparent;
    outline: 0;
    -webkit-appearance: none;
    border: 0;
    padding: 0 10px 0 54px;
    border-top-left-radius: 46px;
    border-bottom-left-radius: 46px;
    border: 1px solid #f8f8f8;
    background-color: #f8f8f8;
    border-right-color: #FF1268;
    box-sizing: content-box;
}
.dm-header-box .search-header .btn-search {
    width: 82px;
    height: 100%;
    position: absolute;
    right: 0;
    top: 0;
    background: #FF1268;
    line-height: 46px;
    font-size: 16px;
    text-align: center;
    color: #FFF;
    border-radius: 0 27px 27px 0;
    z-index: 11;
    letter-spacing: 4px;
    cursor: pointer;
}
.dm-header-box .search-header .list-search-wrap {
    width: 402px;
    position: absolute;
    left: 0;
    top: 0;
    display: none;
}
.dm-header-box .search-header .list-search {
    width: 374px;
    max-height: 296px;
    overflow: hidden;
    position: relative;
    left: 0;
    margin-top: 55px;
    z-index: 999;
    padding: 0 14px;
    background: #FFF;
    box-shadow: 0 2px 8px 0 rgba(0,0,0,.05);
    border-radius: 4px;
}

//       .order-s{
//     /* 设置宽度高度背景颜色 */
//     height: auto; /*高度改为自动高度*/
//     width:100%;
//     margin-left: 0;
//     background:rgb(189, 181, 181);
//     position: fixed; /*固定在顶部*/
//     top: 0;/*离顶部的距离为0*/
//     margin-bottom: 5px;
    
// }
// .order-s ul{
//     /* 清除ul标签的默认样式 */
//     width: auto;/*宽度也改为自动*/
//     list-style-type: none;
//     white-space:nowrap;
//     overflow: hidden;
//     margin-left: 5%;
//     /* margin-top: 0;          */
//     padding: 0;

// }
// .order-s li {
//     float:left; /* 使li内容横向浮动，即横向排列  */
//     margin-right:2%;  /* 两个li之间的距离*/
//     position: relative;
//     overflow: hidden;
// }

// .order-s li a{
//    /* 设置链接内容显示的格式*/
//     display: block; /* 把链接显示为块元素可使整个链接区域可点击 */
//     color:white;
//     text-align: center;
//     padding: 3px;
//     overflow: hidden;
//     text-decoration: none; /* 去除下划线 */
    
// }
// .order-s li a:hover{
//     /* 鼠标选中时背景变为黑色 */
//     background-color: aqua;
// }
// .order-s ul li ul{
//     /* 设置二级菜单 */
//     margin-left: -0.2px;
//     background:rgb(189, 181, 181);
//     position: relative;
//     display: none; /* 默认隐藏二级菜单的内容 */

// }
// .order-s ul li ul li{
//     /* 二级菜单li内容的显示 */
    
//     float:none;
//     text-align: center;
// }
// .order-s ul li:hover ul{
//     /* 鼠标选中二级菜单内容时 */
//     display: block;
// }

//  .s1{
//    font-size: 20px;
//  }
//  .s2{
//    position: absolute;
//    right: -427px;
//  }
//  .s3{
//     position: absolute;
//    right: -500px;
//  }
//  .s4{
//        position: absolute;
//    right: -800px;
//    font-size: 20px;
//  }
 .my-autocomplete {
  li {
    line-height: normal;
    padding: 7px;

    .name {
      text-overflow: ellipsis;
      overflow: hidden;
    }
    .addr {
      font-size: 12px;
      color: #b4b4b4;
    }

    .highlighted .addr {
      color: #ddd;
    }
  }
  
}
//轮播图
.order-head{
  width: 1800px;
 
  border: 1px solid red;
  margin: 0 auto;
  padding: 0;
}
 .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 200px;
    height: 500px;
    margin: 0;
  }

  
  //中部
  .category{
    display: flex;
    justify-content: space-between;
    font-size: 20px;
    font-family: "\5FAE\8F6F\96C5\9ED1";
    margin-top: 15px!important;
    padding: 22px  22px ;
    width: 1750px;
    height: 150px;
    margin: 20px auto;
    border: 1px solid #EBEBEB;
    zoom: 1;
    
  }
  .category__list{
    float: left;
    display: block;
    margin: 20px;
    padding: 5px;
    width: 120px;
 
    text-align: center;
  }
  .category__icon__ych{
   background-position: 0 0;
  }
  .category__icon {
    display: block;
    width: 48px;
    height: 48px;
    margin: 0 auto;
    background: url(//img.alicdn.com/tfs/TB1U9R8GY9YBuNjy0FgXXcxcXXa-146-1822.png) no-repeat;
    background-size: 100% auto;
  }
  .category__icon__gjhj{
        background-position: 0 -64px;
  }
  .category__icon__tyjj{
      background-position: 0 -120px;
  }
  .category__icon__qz{
    background-position: 0 -180px;
  }
  .category__icon__zlxx{
    background-position: 0 -240px;
  }
.category__icon__yyh{
   background-position: 0 -297px;
}
.category__icon__xsxq{
   background-position: 0 -360px;
}
 .category__icon__wdbl{
    background-position: 0 -420px;
 }
 .category__icon__dm{
    background-position: 0 -480px;
 }
 .category__icon__lyzl{
    background-position: 0 -540px;
 }
  .category__info{
    font-size: 16px;
    color: #111;
    text-align: center;
  }
  
a{
  
  text-decoration: none;
}

 
.order-cun{
  width: 1800px;
  height: 500px;
  position: relative;
    margin: 0 auto;
    padding: 22px 0 30px 0;
  border: 1px solid #eeddee;
  margin-top: 15px;
}
.head{
      display: flex;
      justify-content:space-between;
    
    margin: 10 auto;
    height: 200px;
     
    font-size:30px;
}

  
  .el-aside {
    background-color: #D3DCE6;
    color: #333;
    text-align: center;
    line-height: 300px;
  }
  
  .el-main {
    background-color: #E9EEF3;
    color: #333;
    
   
  }
  
   .el-container {
    margin-bottom: 40px;
  }
  
  .el-container:nth-child(5) .el-aside,
  .el-container:nth-child(6) .el-aside {
    line-height: 260px;
  }
  
  .el-container:nth-child(7) .el-aside {
    line-height: 320px;
  }
  .image{
    float: left;
  }
  .box-left{
    width: 370px;
    height: 130px;
    position: absolute;
    bottom: 10px;
    left: 0;
    padding: 17px 10px;
    background-color: rgba(0,0,0,.5);
  }
  .title{
    height: 45px;
    font-size: 28px;
    color: #fff;
    margin-top: 10px;
    
      
   
  }
  .details{
        margin-left: -200px;
    font-size: 28px;
    color: #fff;

  }
  
  .min{
    display: flex;
    justify-content: space-evenly;
    border: 1px solid #ebebee;
  }
.min2{
  float: left;
  width: 280px;
   border: 1px solid #ebebeb;
}
.min3{
  float: left;
  font-size:20px ;
 
}
.min4{
  color: #9B9B9B;
  float: left;
}
.min5 a{
  float: left;
  font-size: 20px;
  color:red;
}
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



// a:link{
//   color: #111;
// }
a:hover{
  color: red;
}


</style>