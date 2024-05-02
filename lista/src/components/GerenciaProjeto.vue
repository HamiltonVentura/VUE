<template>
  <div class="GerenciaProjeto">
    <h1>Cadastro de Tarefas</h1>
    <input v-model="novaTarefa" placeholder="Digite uma nova tarefa">
    <button @click="adicionarTarefa">Adicionar</button>

    <ul>
      <li v-for="(tarefa, index) in tarefas" :key="index">
        {{ tarefa }}
        <button @click="removerTarefa(index)">Remover</button>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'GerenciaProjeto',
  data() {
    return {
      novaTarefa: '',
      tarefas: []
    }
  },
  methods: {
    adicionarTarefa() {
      if (this.novaTarefa.trim() !== '') {
        this.tarefas.push(this.novaTarefa);
        this.novaTarefa = '';
      }
    },
    removerTarefa(index) {
      this.tarefas.splice(index, 1);
    }
  }
}
</script>

<style scoped>

</style>
