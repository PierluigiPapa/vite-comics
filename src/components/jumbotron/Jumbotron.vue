<script>
export default {
  name: 'Jumbotron',
};
</script>

<template>
  
<div class="jumbo"></div>

</template>
  
<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;

.jumbo {
  background-image: url('img/jumbotron.jpg');
  background-size: cover;
  min-height: 500px;
}

h1 {
  color: white;
  padding-top: 50px;
  margin-left: 70px;
  padding-left: 60px;
}
</style>