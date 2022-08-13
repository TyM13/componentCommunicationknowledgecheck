<template>
  <div>
    <section>
      <button @click="selection">CLick Me</button>
    </section>
    <h3>{{ user[`name`] }}</h3>
    <p>{{ user[`age`] }}</p>
    <p>is premium {{ user[`is_premium`] }}</p>
  </div>
</template>

<script>
export default {
  methods: {
    selection() {
      this.$emit(`user_clicked`, this.user[`name`]);
    },
  },

  props: {
    user: Object,
  },
};
</script>

<style scoped>
</style>