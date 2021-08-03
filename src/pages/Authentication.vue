<template>
    <div class="auth">
        <h1>Введите номер телефона</h1>
        <input
        id="authung"
        type="text"
        class='from'
        >
        <button type="button" class="btn btn-outline-light" @click="$router.push({ name: 'films' })">Авторизация</button>
        <h1 class="card-body">Returned Id: {{articleId}}</h1>
        
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
    card-body {
      color: #fff;
    }
    }
    
</style>
<script>
    import axios from "axios";

export default {
  name: "post-request-async-await",
  data() {
    return {
      articleId: null
    };
  },
  async created() {
    // POST request using axios with async/await
    const phone = {phone:"89175184542"};
    const response = await axios.post("http://localhost:3000/phone", phone);
    this.articleId = response.data.message;
  }
};
</script>