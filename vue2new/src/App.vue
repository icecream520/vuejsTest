<template>
  <div id="app">
  <div class="container"><!--//bootstrap内容区域-->
    <nav class="navbar navbar-dark bg-inverse navbar-fixed-top"><!--//bootstrap设置nav元素为导航栏,设置上部填充满-->
      <router-link to="/" class="navbar-brand text-success">简读</router-link><!--//设置路由路径为根目录-->
      <ul class="nav navbar-nav"><!--//设置导航栏 设置ul为导航栏组件内的列表元素-->
        <li class="nav-item">
          <router-link to="/home" class="nav-link"><!--//设置路由-->
            <i class="fa fa-home"></i> Home
          </router-link>
        </li>
    <li class="nav-item">
      <a class="nav-link" href="#"><i class="fa fa-flag"></i>Hot</a>
    </li>
      </ul>
    <form class="form-inline float-xs-right">//form内联
        <input class="form-control" type="text" placeholder="搜索公众号/文章"/>
      <router-link to="/serach"><i class="fa fa-search btn btn-outline-success" @click=""></i></router-link>
      <i class="fa fa-user-o btn btn-outline-success"></i>
    </form>
    </nav>
  </div>
    <div class="container" style="margin-top:80px">
      <div class="row">
        <div class="col-xs-12 col-md-3 push-md-9 col-xl-3 push-xl-9"><!--//小型占12格中型占3格 左边的向右push9个位置-->
          <sidebar>

          </sidebar>
        </div>
        <div class="col-xs-12 col-md-9 pull-md-3 col-xl-9 pull-xl-3"><!--//右边的往左3个位置-->
          <router-view>

          </router-view>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
import Sidebar from'./components/Sidebar.vue'

 export default{
components:{//导入导出组件
'sidebar':Sidebar;
}
    }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
