<template>
  <div id="panel">
    <Tile title_tile="Vos news" bg_color="fuchsia"/>
    <Tile title_tile="Agenda" bg_color="fuchsia"/>
    <Tile title_tile="Paramètres" bg_color="fuchsia"/>
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