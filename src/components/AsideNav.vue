<template>
  <el-row class="left_aside">
    <el-row class="header_logo">LOGO</el-row>
    <el-menu
      default-active="$route.path"
      class="el-menu-vertical-demo"
      router
      active-text-color="#3399FF"
      unique-opened
    >
      <el-menu-item index="1">
        <!-- <img src="../assets/image/yy.png" v-if="$route.path != '/1'" /> -->
        <img src="../assets/image/yy1.png" />
        <span slot="title">医院管理</span>
      </el-menu-item>
      <el-menu-item index="2">
        <!-- <img src="../assets/image/cp.png" /> -->
        <img src="../assets/image/cp1.png" />
        <span slot="title">产品管理</span>
      </el-menu-item>
      <el-menu-item index="3">
        <!-- <img src="../assets/image/ys.png" /> -->
        <img src="../assets/image/ys1.png" />
        <span slot="title">医生管理</span>
      </el-menu-item>
      <el-menu-item index="4">
        <!-- <img src="../assets/image/db.png" /> -->
        <img src="../assets/image/db1.png" />
        <span slot="title">代表管理</span>
      </el-menu-item>
      <el-submenu index="5">
        <template slot="title">
          <!-- <img src="../assets/image/qygl.png" /> -->
          <img src="../assets/image/qygl1.png" />
          <span>区域管理</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="5-1">区域分配</el-menu-item>
          <el-menu-item index="5-2">申请记录</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-menu-item index="6">
        <!-- <img src="../assets/image/qyjl.png" /> -->
        <img src="../assets/image/qyjl1.png" />
        <span slot="title">区域经理</span>
      </el-menu-item>
      <el-menu-item index="7">
        <!-- <img src="../assets/image/zbgl.png" /> -->
        <img src="../assets/image/zbgl1.png" />
        <span slot="title">中标管理</span>
      </el-menu-item>
      <el-submenu index="8">
        <template slot="title">
          <!-- <img src="../assets/image/qy.png" /> -->
          <img src="../assets/image/qy1.png" />
          <span>签约管理</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="8-1">签约审批</el-menu-item>
          <el-menu-item index="8-2">签约档案</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-menu-item index="9">
        <!-- <img src="../assets/image/bfhy.png" /> -->
        <img src="../assets/image/bfhy1.png" />
        <span slot="title">拜访会议</span>
      </el-menu-item>
      <el-menu-item index="10">
        <!-- <img src="../assets/image/jj.png" /> -->
        <img src="../assets/image/jj1.png" />
        <span slot="title">奖金计算</span>
      </el-menu-item>
      <el-menu-item index="11">
        <!-- <img src="../assets/image/yjbg.png" /> -->
        <img src="../assets/image/yjbg1.png" />
        <span slot="title">业绩报告</span>
      </el-menu-item>
      <el-menu-item index="12">
        <!-- <img src="../assets/image/zlzx.png" /> -->
        <img src="../assets/image/zlzx1.png" />
        <span slot="title">资料中心</span>
      </el-menu-item>
      <el-menu-item index="13">
        <!-- <img src="../assets/image/qx.png" /> -->
        <img src="../assets/image/qx1.png" />
        <span slot="title">权限管理</span>
      </el-menu-item>
      <el-menu-item index="14">
        <!-- <img src="../assets/image/sz.png" /> -->
        <img src="../assets/image/sz1.png" />
        <span slot="title">系统设置</span>
      </el-menu-item>
    </el-menu>
  </el-row>
</template>
<script>
export default {
  name: "asideNav",
  date() {
    return {};
  },
  methods: {
    handleOpen() {
      //   console.log(key, keyPath);
    },
    handleClose() {
      //   console.log(key, keyPath);
    }
  }
};
</script>
<style>
.left_aside .el-menu {
  border: none;
}
.left_aside .el-menu .el-menu-item {
  border-left: 3px solid #fff;
}
.left_aside .el-menu .el-menu-item.is-active {
  border-left: 3px solid #3399ff;
}
.left_aside .el-menu .el-icon-arrow-down {
  font-size: 16px;
}
/* .left_aside .el-menu-item,
.left_aside .el-submenu__title {
  display: -webkit-flex;
  display: flex;
  align-items: center;
} */
</style>
<style scoped>
.left_aside {
  background: #fff;
  height: 100%;
  z-index: 99;
}
.header_logo {
  font-weight: bold;
  font-size: 30px;
  text-align: center;
  height: 60px;
  line-height: 60px;
}
.el-menu-vertical-demo {
  height: calc(100% - 60px);
  box-shadow: 2px 5px 6px 0px rgba(218, 218, 218, 1);
}
.el-menu-item img,
.el-submenu__title img {
  margin-right: 8px;
  width: 20px;
  vertical-align: text-top;
}
</style>
