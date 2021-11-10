<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <button @click="openModal()">Press me</button>
    <Modal ref="modal">
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Atque, nemo dignissimos odit doloremque provident quibusdam ad maiores fuga recusandae facilis nisi? Facilis doloremque eaque dolores dignissimos voluptatibus ratione molestias error!</p>
    </Modal>
  </div>
</template>

<script>
import Modal from './components/Modal.vue'

export default {
  name: 'App',
  components: {
    Modal
  },
  methods:{
    openModal(){
      this.$refs.modal.show();
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
