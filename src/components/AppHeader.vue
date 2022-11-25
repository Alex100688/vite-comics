<script>


export default {
  components:{
   
  },
  data() {
    return {
    choiceComic:[
        'CHARACHTERS',
        'COMICS',
        'MOVIES',
        'TV',
        'GAMES',
        'COLLECTIBLES',
        'VIDEOS',
        'FANS',
        'NEWS',
        'SHOP'
     ]
    }
  }
}
</script>

<template>
  <div class="flex-header">
    <img src="../assets/dc-logo.png" alt="">
    <nav class="header-nav">
      <ul v-for="link in choiceComic" >
        <li><a href="">{{link}}</a></li>
      </ul>
    </nav>
  </div>
  <div class="header-bottom">
    <div>
       Content goese here
    </div>
  </div>  
</template>

<style scoped>
  .flex-header{
    display: flex;
    margin-top: 1.875rem;
    justify-content: space-around;
    align-items: center;
    
  }
  img{
    width: 3.75rem;
    height: 3.75rem;
  }
  .header-nav{
    display: flex;
    list-style: none;
  }
  ul{
    list-style: none;
  }
  a{
    text-decoration: none;
    display: inline-block;
    padding: .625rem;
    color: #464646;
  }
  .header-bottom{
    display: flex;
    align-items: center;
    padding-left: 6.25rem;
    margin-top: 2.5rem;
    background-color: var(--second-color);
    color: white;
    height: 6.25rem;
  }
</style>


