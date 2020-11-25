<template>
  <div id="app">
    <div id="main">
    <div id="sidebar">sidebar</div>
    <div id="playlist">playlist</div>
    <div id="ads-space">ads-space</div>
    </div>
    <div id="player">
      <player/>
    </div>
  </div>
</template>

<script>
import player from '@/components/player'
export default {
  components:{
    player
  }
}
</script>

<style>
html, body{
  margin: 0%;
  height: 100%;
  overflow: hidden;
}
#main{
  display: flex;
  flex-direction: row;
  width: 100%;
  background: whitesmoke;
  height: 95vh;
}
#sidebar{
  float: left;
  width: 25%;
  border:thin 1px green
}
#ads-space{
  float: right;
  width: 20%;
  border: solid 2px red;
}
#playlist{
  width: 80%;
  border:solid 2px springgreen;
}
#player{
  position: fixed;
  z-index: 20;
  background: #000;
  left: 0;
  bottom: 0.1em;
  width:100%;
  height: 5em;
}
</style>