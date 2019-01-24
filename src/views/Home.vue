<template>
  <div id="home">
    
  </div>
</template>

<script>
import * as THREE from 'three'

export default {
  name: 'home',
  components: {},
  mounted(){    
    window.THREE = THREE;
    let SCENE = new THREE.Scene();  
    let camera = new THREE.PerspectiveCamera( 75, window.innerWidth / window.innerHeight, 0.1, 1000 );
    let renderer = new THREE.WebGLRenderer();
    renderer.setSize( window.innerWidth, window.innerHeight );
    document.querySelector('#home').appendChild( renderer.domElement );
  },
};
</script>
<style lang="scss">
  #home{
    canvas{
      display:block
    }
  }
</style>