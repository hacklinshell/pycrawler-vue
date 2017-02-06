<template>
  <el-row class="content">
    <el-col :xs="24" :sm="{span: 6,offset: 9}">
      <span class="title">欢迎登录</span>
            <span class="title">福</span>

      <el-row>
        <el-input v-model="account" placeholder="账号" type="text"> </el-input>
        <el-input v-model="password" placeholder="密码" type="password"></el-input>
        <el-col :span="12">
             <el-button type="primary" :click="btnSubmitForm('register')">注册</el-button>
        </el-col>
        <el-col :span="12">
            <el-button type="primary" :click="btnSubmitForm('login')" >登录</el-button>
        </el-col>
      </el-row>
    </el-col>
  </el-row>
</template>

<script>
    export default {
        name: 'login',
        data() {
            return {
                account: '',
                password: ''
            }
        },
        methods: {
            btnSubmitForm: function(form) {
                if (form == 'login') {

                } else if (form == "register") {

                } else if (form == "forget-pwd") {

                }
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style type="text/css" scoped>
    .el-row content {
        padding: 16px
    }
    
    .title {
        font-family: "Helvetica";
        font-size: 28px
    }
    
    .el-input {
        margin: 12px 0
    }
    
    .el-button {
        width: 95%;
    }
</style>