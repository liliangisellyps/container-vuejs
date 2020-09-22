<template>
  <div id="app">
    <Container>
      <p slot="title" class="title">Usuários</p>
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
    background-color: #fab400;
    box-shadow: 0px 3px 6px #00000029;
    border: none;
    border-radius: 15px;
    padding: 10px 22.5px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 24px;
    font-family: 'Open Sans', sans-serif;
    color: #383838;
    opacity: 1.0;
  }
  .button:hover {
    opacity: 0.9;
    cursor: pointer;
  }
  table {
    border-spacing: 0;
    border-collapse: collapse;
    border: 1px solid #9A9A9A;
    margin-top: 22.5px;
  }
  th {
    text-align: left;
    font-weight: 100;
    background-color: #fff;
    border-bottom: 1px solid #D6D6D6;
  }
  th, td {
    padding: 15px;
    font-weight: 600;
    font-size: 22px;
  }
  tr:nth-child(even) {
    background-color: #fff;
  }
  tr:nth-child(odd) {
    background-color: #F2F2F2;
  }
</style>
