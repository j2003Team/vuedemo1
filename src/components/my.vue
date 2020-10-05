<template>
    <!--此部分为视图-->
    <div>
        <form>
            UserName:<input type="text" name = "username" v-model="userInfo.username"/><br/>
            password:<input type="text" name = "password" v-model="userInfo.password"/><br/>
            age:<input type="text" name = "age"  v-model="userInfo.age"/><br/>
            <button @click="login" >LOGIN</button>
        </form>
        <div>

        <h2> hjjkkklll</h2>
        
        </div>
    </div>

  
</template>

<script>
export default {
    name:'MyVue2',
    
    data(){
        return{
            userInfo:{'username':'','password':'','age':18}
        }
    },
    methods:{
        login:function() {

            alert(userInfo.username+"--"+userInfo.password+"=="+userInfo.age);
        }

    }
}
</script>
<style  scoped>
/*css样式 */
</style>