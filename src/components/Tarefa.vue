<template>
  <div>
    <ul>
      <li v-for="(tarefa) in tarefas" :key="tarefa">
        <p v-if="tarefa.estaCompleta === true" class="completa">ID: {{ tarefa.id }} - Descrição: {{ tarefa.descricao }} => Completa
        </p>
        <p v-else class="incompleta">ID: {{ tarefa.id }} - Descrição: {{ tarefa.descricao }} => Incompleta</p>
      </li>
    </ul>
  </div>   
</template>

<script>
  export default {
    name: 'Tarefas',
    data:function() {
        return {
          tarefas : [
              { id: 1, descricao:'Descrição da tarefa #1', estaCompleta: true },
              { id: 2, descricao:'Descrição da tarefa #2', estaCompleta: false },
              { id: 3, descricao:'Descrição da tarefa #3', estaCompleta: false },
              { id: 4, descricao:'Descrição da tarefa #4', estaCompleta: true },
              { id: 5, descricao:'Descrição da tarefa #5', estaCompleta: false },
              { id: 6, descricao:'Descrição da tarefa #6', estaCompleta: true }
          ]
        };
    }
  }
</script>

<style scoped>
ul {
  list-style-type: none;
}

li{
  margin-bottom: 20px;
}

.completa{
  color: green;
  font-weight: bold;
}

.incompleta{
  color: red;
}
</style>