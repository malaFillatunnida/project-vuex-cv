<template> 
  <div class="col-md-6"> 
    <div class="card"> 
      <div class="card-body"> 
          <h2>Summary</h2><hr>
          <p v-for="row in listAgenda" :key="row">{{ row.summary }}</p>

          <h2>Skill Highlights</h2><hr>
          <ul>
          <li><p v-for="row in listAgenda" :key="row">{{ row. skillHighlight }}</p></li>
          </ul>

          <h2>Organization Experience</h2><hr>
         <ul>
          <li><p v-for="row in listAgenda" :key="row">{{ row. organizationExperience1 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row. organizationExperience2 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row. organizationExperience3 }}</p></li>
          </ul>

          <h2>Educational Background</h2><hr>
          <ul>
          <li><p v-for="row in listAgenda" :key="row">{{ row.educationalBackground1 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row.educationalBackground2 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row.educationalBackground3 }}</p></li>
          </ul>
          
          <h2>Achievement</h2><hr>
          <ul>
          <li><p v-for="row in listAgenda" :key="row">{{ row.achievement1 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row.achievement2 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row.achievement3 }}</p></li>
          </ul>
      </div> 
    </div> 
  </div> 
</template>  
<script>  
export default {  
  name: 'AgendaInput',  
  computed: {  
    listAgenda() {  
      return this.$store.state.listAgenda  
    }  
  }  
}  
</script>

<style scoped>
.card-body {
background-color: rgb(82, 159, 221);
}
</style>