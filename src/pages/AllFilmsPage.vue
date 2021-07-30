<template>
  <div class="films-page container">
    <h2>Введите ссылку для продолжения работы </h2>
    <films-list :films="films" />
  </div>
</template>

<script>
import FilmsList from '../components/FilmsList'
import films from '../mocks/films'


export default {
  components: { FilmsList },
  data() {
    return {
      films
    }
  }
}
</script>

<style lang="scss" scoped>
h2 {
  font-size: 40px;
  color:#ffffff;
  margin-bottom: 30px;
}
</style>