<template>
  <div>
    <h1>模拟登录</h1>
    用户名：<input type="text" placeholder="请输入用户名" v-model='username'><br>
    密码：<input type="text" placeholder="请输入密码" v-model="password">
    <br>
    <button @click.prevent='login'>登录</button>
    <button @click='reset'>重置</button>
  </div>
</template>

<script>
export default {
data(){
  return{
    username:'',
    password:''
  }
},
methods:{
  login(){
    if(!this.username){
      alert('用户名不能为空')
    }
    if(!this.password){
      alert('密码不能为空')
    }
    console.log('需要送请求',this.username,this.password);
  },
  reset(){
    this.name='',
    this.password=''
  }
}
  
    }
  

</script>

<style>

</style>