<template>
  <div class="login">
     <el-tabs v-model="activeName" @tab-click="handleClick">
    <el-tab-pane label="登录" name="first">登录</el-tab-pane>
    <el-tab-pane label="注册" name="second">注册</el-tab-pane>
  </el-tabs>
  </div>
</template>
<script>
export default {
  name: "login",
  data() {
    return {
      activeName: 'first'
    }
  },
  methods: {
    handleClick(tab,event){
      console.log(tab,event);
    }
  },
};
</script>
<style lang="scss" scoped>
.login {
  height: 100vh;
  background-color: #6666;
}
</style>
