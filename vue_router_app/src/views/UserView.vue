<template>
    <h1>Usuários</h1>
    <button @click="login()" >Logar</button>
</template>

<script setup>
import { useRouter } from 'vue-router';

const router =useRouter();

function login(){
    console.log('logou');
     router.push('/about')  ;
  
}
</script>