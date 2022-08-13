<template>
  <div>
    <h3>{{user[`name`]}}</h3>
    <p>{{user[`age`]}}</p>
    <p>is premium {{user[`is_premium`]}}</p>
  </div>
</template>

<script>
export default {
props: {
  user: Object,

  
},
};
</script>

<style scoped>
</style>