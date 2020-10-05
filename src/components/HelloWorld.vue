<template>
 <div>
   <!--此部分为视图-->
   <form>
      username:<input type="text" name="username" v-model="userInfo.username"/><br/>
      password:<input type="text" name="password" v-model="userInfo.password"/><br/>
      age:<input type="text" name="age" v-model="userInfo.age"/><br/>
      <button @click="login">Login</button>

   </form>
 </div>
 
</template>

<script>
//编写js行为

export default{
  
  name:'MyVue',
  data(){
      return{

        userInfo:{'username':'','password':'','age':18}
      }
     
  },
   methods:{

        login:function(){
          
          alert(this.userInfo.username);
        }
      }


}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/*css样式*/
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
