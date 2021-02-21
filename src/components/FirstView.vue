<template>
  <div id="NOTE" @click="countUp">
    <div class="notes">
      A
    </div>
  </div>
</template>

<script>
export default {
  name: 'FirstView',
  data () {
    return {
      notes: ['A', 'B♭', 'B', 'C', 'D♭','D', 'E♭', 'E', 'F', 'G♭', 'G', 'A♭' ]
    }
  },
  methods: {
    countUp() {
      const number = Math.floor(Math.random() * this.notes.length);
      const selectedImg = this.notes[number];
      const note =  document.querySelector(".notes")
      note.innerHTML = selectedImg;
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .notes{
    font-size: 140px;
    cursor: pointer;
    height: 200px;
    line-height: 200px;   
    margin-top: 200px; 
  }
</style>
