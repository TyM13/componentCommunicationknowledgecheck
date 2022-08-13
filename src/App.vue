<template>
  <div id="app">

  <small-user-profile v-for="user_obj in users" :key="user_obj[`id`]" :user="user_obj"></small-user-profile>
  </div>
</template>

<script>
import SmallUserProfile from '@/components/SmallUserProfile.vue'

export default {

  data() {
    return {
      users: [
        {
          name: `Ty`,
          age: 25,
          is_premium: true,
          id: 1,
        },
        {
          name: `Tyler`,
          age: 20,
          is_premium: false,
          id: 4,
        },
      ],
    };
  },

  name: 'App',
  components: {
 SmallUserProfile,
  }

  
}
</script>

<style>

</style>
