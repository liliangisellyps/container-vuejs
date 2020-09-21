<template>
  <div id="app">
    <div class="container">
      <h1>TODO VUE!</h1>
      <input
        class="input"
        v-model="newToDo"
      />
      <button class="add-button">Add</button>
      <ul style="list-style-type: none;">
        <li v-for="(todo, i) in existingToDo" v-bind:key="todo.id">
          <span>
            {{i+1}}: {{todo.text}}
          </span>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>

export default {
  name: 'App',
  data(){
    return {
      newToDo: '',
      existingToDo: [
        {text: 'cry', id:0},
        {text: 'sleep', id: 1},
        {text: 'eat', id: 2}
      ]
    }
  },
  method: {
    add(){
      this.existingToDo.push({
        text: this.newToDo,
        id: new Date().valueOf()
      }),
      THIS.
    }
  }
}
</script>

<style>

</style>
