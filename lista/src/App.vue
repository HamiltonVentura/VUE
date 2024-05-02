<template>
  <h1> Bem vindos primeiro Teste com Vue.jS</h1>
  <h3>{{ dados.toLocaleUpperCase()}}</h3>

  <ul>
    <li><a href="#">Início</a></li>
    <li><a href="#">Cadastro</a></li>
  </ul>
  <HelloWorld/>
  <GerenciaProjeto/>


</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import GerenciaProjeto from './components/GerenciaProjeto.vue';

export default {
  components:
  {
    HelloWorld,
    GerenciaProjeto
  },
  data() {
      return {
        dados: "bom dia!"
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
  h3 {
    margin: 40px 0 0;
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


<!-- <template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Bem Vindo a Lista de Tarefas"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
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
</style> -->
