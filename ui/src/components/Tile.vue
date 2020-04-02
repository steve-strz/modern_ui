<template>
  <div id="tile">
    <div class="container" :style="{backgroundColor:color, boxShadow: color, height: height, width: width}">
        <div class="top">
            <div class="title">
                {{title}}
            </div>
        </div>
        <div class="middle">
            
        </div>
        <div class="bottom">
            
        </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'tile',
  data(){
      return{
          title: this.title_tile,
          color: this.bg_color,
          height: this.height_tile,
          width: this.width_tile
      }
  },
  components: {
    
  },
  props:['title_tile', 'bg_color', 'height_tile', 'width_tile'],
  methods:{
      
  }
}
</script>

<style>
#tile{
    display:flex;
    flex-direction: row;
    justify-content: center;
    margin: 5px;
}

.container{
    display:flex;
    flex-direction: column;
    height: 400px;
    width: 250px;
    background-color: rgb(101, 193, 221);
    transition: width 0.15s, height 0.15s;
    box-shadow: 5px 5px pink;
}
.container:hover{
    height: 410px;
    width: 260px;
}

.top{
    display:flex;
    flex-direction: row;
    flex:1;
}
.middle{
    display:flex;
    flex-direction: row;
    flex:1;
}
.bottom{
    display:flex;
    flex-direction: row;
    flex:1;
}

.title{
    margin: 8%;
    font-size: 20px;
}
</style>