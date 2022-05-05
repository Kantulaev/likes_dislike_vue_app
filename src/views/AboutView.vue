<template>
  <div class="about">
    <h1>This is an about page 123</h1>
    <h2>Лайков: {{likes}}</h2>
    <h2>Дизлайков: {{dislikes}}</h2>
    <button v-on:click="LikesUp">Like</button>
    <button @click = "DislikesUp">Dislike</button>
  </div>
</template>

<script>
export default {
  data(){
    return{
      likes: 0,
      dislikes: 0
    }
  },
  
  methods: {
    LikesUp(){
      this.likes += 1;
    },
    DislikesUp(){
      this.dislikes += 1;
    }
  }

}
</script>

<style>

</style>