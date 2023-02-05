<template>
    <ul class="list-group">
  <li class="list-group-item" v-for="item in cart" :key="item.id">
    <div class="row">
        <div class="media col-9">
    <img width="40px" :src="item.gambar" class="mr-3" :alt="item.nama"/>
    <div class="media-body">
        <p class="mt-0">{{item.nama}}</p>
        <button class="btn-qt btn btn-sm btn-secondary">-</button>
        x {{ item.qty }}
        <button class="btn-qt btn btn-sm btn-secondary">+</button>
    </div>
  </div>
  <button type="button" class="btn-close col-3" data-bs-dismiss="modal" aria-label="Close"></button>
    </div>
    
  
</li>  
</ul>
</template>
<script>

export default{
   
}
</script>
<style>
.btn-qt{
    border-radius: 50%;
    width: 30px;
}
.media-body{
    text-align: left;
}
.media img{
    width: 50%;
}
.card{
    padding: 20px;
}
</style>