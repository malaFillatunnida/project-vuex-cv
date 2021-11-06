<template> 
  <div id="app" class="container"> 
  <div class="row py-4">
    <agenda-show/>
    <agenda-input/>
  </div>
  <div class="row py-4"><br>
    <agenda-input2/>
  </div>
  </div>
</template> 
 
<script> 
import AgendaShow from './components/AgendaShow.vue' 
import AgendaInput from './components/AgendaInput.vue' 
import AgendaInput2 from './components/AgendaInput2.vue'
 
export default { 
  name: 'App', 
  components: {
    AgendaShow,
    AgendaInput, 
    AgendaInput2
  } 
} 
</script> 
