<template>
  <div class="container">
      <div class="header">
          <slot name="title"></slot>
          <slot name="action"></slot>
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
    font-family: 'Open Sans', sans-serif;
    padding: 30px;
    border-radius: 12px;
  }
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid #a6a6a6;
  }
  
</style>
