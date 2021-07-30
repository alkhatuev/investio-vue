<template>
    <div class="auth">

        <h1>Введите номер телефона</h1>
       
        <input
        id="authung"
        type="text"
        class='from'
        >
        <button type="button" class="btn btn-outline-light" @click="$router.push({ name: 'films' })">Авторизация</button>
        
    </div>


</template>

<style lang="scss" scoped>
    .auth {
        display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    h1 {
      color: #fff;
      font-size: 70px;
      margin-bottom: 20px;
    }
    input {
       font-size: 35px;
      margin-bottom: 20px; 
        
    }
    button {
    
    }
    }
    
</style>
<script>
    
   


</script>
