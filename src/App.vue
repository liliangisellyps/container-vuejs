<template>
  <div id="app">
    <Container>
      <h2 slot="title">Usuários</h2>
      <button slot="action" class="button">Adicionar</button>
      <table slot="body" style="width:100%">
      <tr>
        <th>Nome</th>
        <th>Campo 1</th>
        <th>Campo 2</th>
        <th>Campo 3</th>
        <th>Campo 4</th>
      </tr>
      <tr>
        <td>Fulano</td>
        <td>Campo 1</td>
        <td>Campo 2</td>
        <td>Campo 3</td>
        <td>Campo 4</td>
      </tr>
      <tr>
        <td>Fulano</td>
        <td>Campo 1</td>
        <td>Campo 2</td>
        <td>Campo 3</td>
        <td>Campo 4</td>
      </tr>
      <tr>
        <td>Fulano</td>
        <td>Campo 1</td>
        <td>Campo 2</td>
        <td>Campo 3</td>
        <td>Campo 4</td>
      </tr>
      <tr>
        <td>Fulano</td>
        <td>Campo 1</td>
        <td>Campo 2</td>
        <td>Campo 3</td>
        <td>Campo 4</td>
      </tr>
    </table>
    </Container>
  </div>
</template>

<script>
import Container from '@/components/Container';

export default {
  name: 'App',
  components: {Container}
}
</script>

<style>
  .button {
    background-color: #fab400; /* Green */
    border: none;
    border-radius: 12px;
    padding: 10px 35px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 20px;
    font-family: 'Open Sans', sans-serif;
  }
  table {
    border-spacing: 0;
    border-collapse: collapse;
    border: 1px solid #b4b4b4;
    margin-top: 15px;
  }
  th {
    text-align: left;
    font-weight: 100;
    background-color: #fff;
    border-bottom: 1px solid #eee;
  }
  th, td {
    padding: 15px;
  }
  tr:nth-child(even) {
    background-color: #fff;
  }
  tr:nth-child(odd) {
    background-color: #eee;
  }
</style>
