<template>
  <h2>кол-во лайков {{likes}}</h2>
  <h2>кол-во дизлайков {{dislikes}}</h2>
 <button @click="likesCounter">лайки</button>
 <button @click="dislikesCounter">дизлайки</button>
     
</template>
<script>
export default {
    data(){
        return{
            likes: 0,
            dislikes: 0
        }
    },
    methods:{
       likesCounter(){
        this.likes += 1
       },
       dislikesCounter(){
        this.dislikes += 1
       }
    }
}
</script>
<style>

</style>