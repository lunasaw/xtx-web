<template>
  <!-- 轮播区域 -->
  <div class="banner">
      <div class="wrapper">
        <!-- 图 -->
        <ul class="pic">
          <li>
            <a href="#"><img src="@/assets/images/banner1.png" alt="" /></a>
          </li>
          <li>
            <a href="#"><img src="@/assets/images/banner1.png" alt="" /></a>
          </li>
        </ul>
        <!-- 侧导航 -->
        <div class="subnav">
          <ul>
            <li>
              <div>
                <span><a href="#">生鲜</a></span>
                <span><a href="#">水果</a><a href="#">蔬菜</a></span>
              </div>
              <i class="iconfont icon-arrow-right-bold"></i>
            </li>
            <li>
              <div>
                <span><a href="#">美食</a></span>
                <span><a href="#">面点</a><a href="#">干果</a></span>
              </div>
              <i class="iconfont icon-arrow-right-bold"></i>
            </li>
            <li>
              <div>
                <span><a href="#">餐厨</a></span>
                <span><a href="#">数码产品</a></span>
              </div>
              <i class="iconfont icon-arrow-right-bold"></i>
            </li>
            <li>
              <div>
                <span><a href="#">电器</a></span>
                <span
                  ><a href="#">床品</a><a href="#">四件套</a
                  ><a href="#">被枕</a></span
                >
              </div>
              <i class="iconfont icon-arrow-right-bold"></i>
            </li>
            <li>
              <div>
                <span><a href="#">居家</a></span>
                <span
                  ><a href="#">奶粉</a><a href="#">玩具</a
                  ><a href="#">辅食</a></span
                >
              </div>
              <i class="iconfont icon-arrow-right-bold"></i>
            </li>
            <li>
              <div>
                <span><a href="#">洗护</a></span>
                <span
                  ><a href="#">洗发</a><a href="#">洗护</a
                  ><a href="#">美妆</a></span
                >
              </div>
              <i class="iconfont icon-arrow-right-bold"></i>
            </li>
            <li>
              <div>
                <span><a href="#">孕婴</a></span>
                <span><a href="#">奶粉</a><a href="#">玩具</a></span>
              </div>
              <i class="iconfont icon-arrow-right-bold"></i>
            </li>
            <li>
              <div>
                <span><a href="#">服饰</a></span>
                <span><a href="#">女装</a><a href="#">男装</a></span>
              </div>
              <i class="iconfont icon-arrow-right-bold"></i>
            </li>
            <li>
              <div>
                <span><a href="#">杂货</a></span>
                <span><a href="#">户外</a><a href="#">图书</a></span>
              </div>
              <i class="iconfont icon-arrow-right-bold"></i>
            </li>
            <li>
              <div>
                <span><a href="#">品牌</a></span>
                <span><a href="#">品牌制造</a></span>
              </div>
              <i class="iconfont icon-arrow-right-bold"></i>
            </li>
          </ul>
        </div>
        <!-- 指示器 -->
        <ol>
          <li class="current"><i></i></li>
          <li><i></i></li>
          <li><i></i></li>
        </ol>
      </div>
    </div>

</template>

<script>
export default {

}
</script>

<style scoped>
/* 头部导航 */
.header {
  display: flex;
  margin: 22px auto;
}
.header .logo {
  margin-right: 40px;
  width: 200px;
  height: 88px;
  background-color: pink;
}
.header .logo a {
  display: block;
  width: 200px;
  height: 88px;
  background-image: url(~@/assets/images/logo.png);
  font-size: 0;
}
.header .nav {
  margin-top: 33px;
  margin-right: 27px;
}
.header .nav ul {
  display: flex;
}
.header .nav li {
  margin-right: 48px;
}
.header .nav a {
  display: block;
  height: 34px;
}
.header .nav a:hover {
  border-bottom: 2px solid #5EB69C;
}
.header .search {
  display: flex;
  margin-right: 45px;
  margin-top: 33px;
  width: 170px;
  height: 34px;
  border-bottom: 2px solid #F4F4F4;
}
.header .search .icon-search {
  margin-right: 8px;
  font-size: 20px;
  color: #999;
}
.header .search input {
  flex: 1;
}
.header .search input::placeholder {
  color: #ccc;
}
.header .cart {
  position: relative;
  margin-top: 33px;
}
.header .cart .icon-cart-full {
  font-size: 24px;
}
.header .cart i {
  position: absolute;
  /* right: -5px; */
  left: 15px;
  top: 0;
  padding: 0 5px;
  height: 15px;
  background-color: #E26237;
  border-radius: 7px;
  font-size: 12px;
  color: #fffefe;
  line-height: 15px;
}


/* 轮播区域 */
.banner {
  height: 500px;
  background-color: #F5F5F5 ;
}
.banner .wrapper {
  position: relative;
  overflow: hidden;
}
.banner .pic {
  display: flex;
  width: 3720px;
  height: 500px;
}
.banner .pic li {
  width: 1240px;
  height: 500px;
}
.banner .subnav {
  position: absolute;
  left: 0;
  top: 0;
  width: 250px;
  height: 500px;
  background-color: rgba(0,0,0,0.42);
}
.banner .subnav li {
  display: flex;
  justify-content: space-between;
  padding: 0 20px 0 30px;
  height: 50px;
  line-height: 50px;
}
.banner .subnav a,
.banner .subnav i {
  color: #fff;
}
.banner .subnav li span:nth-child(1) {
  margin-right: 14px;
}
.banner .subnav li span:nth-child(2) a {
  margin-right: 5px;
}
.banner .subnav li span:nth-child(2) a {
  font-size: 14px;
}
.banner .subnav li:hover {
  background-color: #00BE9A;
}
.banner ol {
  position: absolute;
  right: 17px;
  bottom: 17px;
  display: flex;
}
.banner ol li {
  cursor: pointer;
  margin-left: 8px;
  padding: 4px;
  width: 22px;
  height: 22px;
  background-color: transparent;
  border-radius: 50%;
}
.banner ol li i {
  display: block;
  width: 14px;
  height: 14px;
  background-color: rgba(255,255,255,0.5);
  border-radius: 50%;
}
.banner ol .current {
  background-color: rgba(255,255,255,0.5);
}
.banner ol .current i {
  background-color: #fff;
}
</style>