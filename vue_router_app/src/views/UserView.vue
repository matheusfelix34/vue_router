<template>
    <h1>Usuários</h1>
    <button @click="login()" >Logar</button>
</template>

<script setup>
import { useRouter } from 'vue-router';

const router =useRouter();

const { params } = router.currentRoute.value;

function login(){
    console.log(params);
     router.push('/about')  ;
  
}
</script>   