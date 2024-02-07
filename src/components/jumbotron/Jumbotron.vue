<script>
export default {
  name: 'Jumbotron',
};
</script>

<template>
  
<div class="jumbo">
  <h1> &#8594; Content goes here &#8592; </h1>
</div>

</template>
  
  <style lang="scss" scoped>
  @use '../../styles/partials/variables.scss' as *;
  
  .jumbo {
    background-color: #1c1c1c;
    min-height: 150px;
  }

  h1 {
    color: white;
    padding-top: 50px;
    margin-left: 70px;
    padding-left: 60px;
  }

  </style>