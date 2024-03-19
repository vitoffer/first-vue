<template>
  <h3>{{ info }} + {{ login }}</h3>
  <p>Anons</p>

  <button type="button" @click="userData()" @mouseover="this.login = 'new text 1'">Отправить</button>
</template>

<script>
export default {
  data() {
    return {
      info: 'infoText',
      login: '123'
    }
  },
  methods: {
    userData() {
      this.info = 'New Text'
    }
  }
}
</script>

<style scoped>
h3 {
  font-weight: lighter;
}

p {
  color: rgb(255, 0, 0);
}
</style>
