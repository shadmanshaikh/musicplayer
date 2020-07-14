<template>
  <div id="app">
    

  <br>
    <div class="shadow p-3 mb-5 bg-white rounded text-dark">
        <h2 class="text-light"> Thunder </h2>
       <button class="btn btn-success btn-sm" @click.prevent="playSound('https://www.talk2trend.com/english/Imagine-Dragons-Thunder.mp3')">
       <span class="fa fa-play-circle-o"></span>Play</button>
      

    </div>

    <br>
    <div class="shadow p-3 mb-5 bg-white rounded text-dark">
        <h2 class="text-light"> See You Again </h2>
       <button class="btn btn-success btn-sm" @click.prevent="playSound('https://www.talk2trend.com/english/see-you-again-ft-charlie-puth.mp3')">
       <span class="fa fa-play-circle-o"></span>Play</button>
      



  </div>
  </div>
</template>

<script>


export default {
  name: 'app',
  methods: {
    
    playSound (sound) {
      if(sound) {
        var audio = new Audio(sound);
        audio.play();
      }
    },
    
  }
}
</script>