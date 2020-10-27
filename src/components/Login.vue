<template>
    <div>
        <input type="text" placeholder="Enter User Name"/> <br><br>
        <input type="password" placeholder="Enter pass"/> <br><br>
        <button v-on:click="getLogin"> LogIn</button>
    </div>
</template>

<script>
export default {
    name:'Login',
    data(){
        return{
            loginForm:{
                username:null,
                password:null
            }
        }
    },
    methods:{
        getLogin(){
            console.log('login');
        }
    }
}
</script>