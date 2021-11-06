<template>
    <div id="mala">
    <div class="border1">
        <div class="head">
           <h1 style="font-family: times new roman;text-align: left;">MALA <br><span> FILLATUNNIDA</span></h1><br>
        </div>
    <img src="https://ajaib-wp-s3-artifact.s3.ap-southeast-1.amazonaws.com/prd/wp-content/uploads/2019/12/wanita-muslimah-inspiratif.jpg" width="300px" height="180px">

    <br><br>

    <h3 style="font-family: times new roman;">BOOTCAMP PARTICIPANTS</h3><hr>
    <h2>PROFILE</h2><hr style="border: 1px dashed">
    <p><b>NAME</b></p>
    <p v-for="row in listAgenda" :key="row">{{ row.name }}</p>
    <p><b>DATE OF BIRTH</b></p>
    <p v-for="row in listAgenda" :key="row">{{ row.date }}</p>
    <p><b>ADDRESS</b></p>
    <p v-for="row in listAgenda" :key="row">{{ row.address }}</p>
    <p><b>WEBSITE</b></p>
    <p v-for="row in listAgenda" :key="row">{{ row.website }}</p>
 
    <h2>AWARDS</h2><hr style="border: 1px dashed">
    <p><b>CHARTER AWARD 2012 </b></p> 
    <p v-for="row in listAgenda" :key="row">{{ row.character }}</p>
    <p><b>INTERFACE DESIGN 2013 </b></p> 
    <p v-for="row in listAgenda" :key="row">{{ row.interface }}</p>

    <h2>CONTACT</h2><hr style="border: 1px dashed">
    <p><b> HOME NUMBER &#x1F3E0;</b></p>
    <p v-for="row in listAgenda" :key="row">{{ row.home }}</p>
    <p><b>PHONE NUMBER &#x1F4DE;</b></p> 
    <p v-for="row in listAgenda" :key="row">{{ row.phone }}</p>
    <p><b>EMAIL &#x1F4E7;</b></p> 
    <p v-for="row in listAgenda" :key="row"><u>{{ row.email }}</u></p>
 
    <h2>SOCIAL</h2><hr style="border: 1px dashed">
    <p><b>TWITTER</b></p>
    <p v-for="row in listAgenda" :key="row">{{ row.twitter }}</p>
    <p><b>FACEBOOOK </b></p>
    <p v-for="row in listAgenda" :key="row">{{ row.facebook }}</p>
    </div>

    <div class="border2">
    <div id="p">
        <h2>Words of Wisdom</h2><hr style="border: 1px dashed">
          <ul>
          <li><p v-for="row in listAgenda" :key="row">{{ row.word1 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row.word2 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row.word3 }}</p></li>
          </ul>
    </div>
<br>
    <div id="p">
        <h2>Summary</h2><hr style="border: 1px dashed">
    <p v-for="row in listAgenda" :key="row">{{ row.summary }}</p>
    </div>
<br> 
    <div id="p">
        <h2>Achievement</h2><hr style="border: 1px dashed">
          <ul>
          <li><p v-for="row in listAgenda" :key="row">{{ row.achievement1 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row.achievement2 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row.achievement3 }}</p></li>
          </ul>
    </div>
<br>
    <div id="p">
        <h2>Life Motivation</h2><hr style="border: 1px dashed">
        <p v-for="row in listAgenda" :key="row">{{ row.life1 }}</p>
        <p v-for="row in listAgenda" :key="row">{{ row.life2 }}</p>
        <p v-for="row in listAgenda" :key="row">{{ row.life3 }}</p>
    </div>
<br>
    <div id="p">
        <h2>Educational Background</h2><hr style="border: 1px dashed">
          <ul>
          <li><p v-for="row in listAgenda" :key="row">{{ row.educationalBackground1 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row.educationalBackground2 }}</p></li>
          <li><p v-for="row in listAgenda" :key="row">{{ row.educationalBackground3 }}</p></li>
          </ul>
    </div><br>
<br>

    </div>
    
    </div>
</template>

<script>  
export default {  
  name: 'AgendaInput2',  
  computed: {  
    listAgenda() {  
      return this.$store.state.listAgenda  
    }  
  }  
}  
</script>


<style scoped>
#mala {
    padding: 20px;
    margin-left: 30px;
}

.border1 {
    border: 1px solid lightgrey;
    padding: 20px;
    width: 350px;
    background-color: lightgrey;
    float: left;
    text-align: right;
}

.border2 {
    border: 1px solid white;
    padding: 20px;
    background-color: white;
    float: left;
    width: 65%;
    height: 894px;
    margin-bottom: 50px;
}

#p {
  background-color: darkgrey;
  padding: 20px;
  height: 310px;
}

h2 {
font-family: 'Times New Roman', Times, serif;
}

</style>