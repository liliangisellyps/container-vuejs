<template>
  <div class="container">
      <div class="header">
          <div class="title"><slot name="title"></slot></div>
          <div class="action"><slot name="action"></slot></div>
      </div>
      <div class="body">
          <slot name="body"></slot>
      </div>
  </div>
</template>

<script>

export default {
  name: 'Container'
}
</script>

<style>
  .container {
    color: #383838;
    font-family: 'Open Sans', sans-serif;
    padding: 30px;
    border-radius: 12px;
  }
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid #707070;
    padding-bottom: 22.5px;
  }
  .title {
    font-weight: bold;
    font-size: 36px;
    margin: 0;
  }  
</style>
