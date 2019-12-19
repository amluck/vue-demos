<template>
  <div class="home">
    <!-- <element-form></element-form> -->
    <!-- <hello-element></hello-element> -->
    <el-container>
      <el-aside width="200px">
        <el-menu router default-active="/table">
          <el-submenu index="/">
            <template slot="title">
              <i class="el-icon-menu"></i>
              <span>数据管理</span>
            </template>
            <el-menu-item index="/form">
              <template slot="title">
                <i class="el-icon-suitcase"></i>
                <span>项目分组</span>
              </template>
            </el-menu-item>
            <el-menu-item index="/table">
              <template slot="title">
                <i class="el-icon-suitcase"></i>
                <span>数据管理</span>
              </template>
            </el-menu-item>
          </el-submenu>
          <el-menu-item index="/about">
            <i class="el-icon-menu"></i>
            <span slot="title">服务管理</span>
          </el-menu-item>
        </el-menu>
        <!-- Aside content -->
      </el-aside>
      <el-container>
        <el-header>
          header
          <!-- Header content -->
        </el-header>
        <el-main>
          <router-view></router-view>
          <!-- Main content -->
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloElement from "@/components/HelloElement.vue";
// import ElementForm from "@/components/ElementForm.vue";

export default {
  name: "home",
  components: {
    // HelloElement,
    // ElementForm
  }
};
</script>
<style>
.el-header,
.el-footer {
  background-color: #b3c0d1;
  color: #333;
  text-align: center;
  line-height: 60px;
}

.el-aside {
  background-color: #d3dce6;
  color: #333;
  text-align: center;
  line-height: 200px;
}

.el-main {
  background-color: #e9eef3;
  color: #333;
  text-align: center;
  line-height: 160px;
}
</style>
