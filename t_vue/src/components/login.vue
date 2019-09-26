<template>
  <div class="d_body">
    <div class="logo"></div>
    <div class="form-item">
      <el-form ref="form" :mode="form">
        <el-row>
          <el-input v-model="form.name" placeholder="邮箱"></el-input>
        </el-row>
        <el-row>
          <el-input v-model="form.password" placeholder="密码" show-password></el-input>
        </el-row>
        <el-button size="medium"   @click="onSubmit" round>登录</el-button>
      </el-form>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      form: {
        name: "",
        password: ""
      }
    };
  },
  methods: {
    onSubmit() {
      console.log(this.form);
    }
  }
};
</script>
<style scoped>
.d_body {
  width: 430px;
  height: 550px;
  top: 50%;
  left: 50%;
  border: 1px solid #fff;
  margin: -300px 0 0 -215px;
  border-radius: 20px;
  overflow: hidden;
  position: absolute;
}
.logo {
  width: 104px;
  height: 104px;
  margin: 50px auto 80px;
  background: url(../../static/f90fd75a0cd8233ec9d90e298e8cb628.jpeg) 0 0
    no-repeat;
  -moz-background-size: 100% 100%;
  background-size: 100% 100%;
}
.form-item {
  position: relative;
  width: 360px;
  margin: 0 auto;
  padding-bottom: 30px;
}

</style>