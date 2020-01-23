<template>
  <div id="panel">
    <Tile title_p="Vos news"/>
    <Tile title_p="Agenda"/>
    <Tile title_p="Paramètres"/>
  </div>
</template>

<script>
import Tile from "./Tile";

export default {
  name: 'panel',
  components: {
    Tile
  }
}
</script>

<style>
#panel{
    display:flex;
    flex-direction: row;
    justify-content: center;
}
</style>