<template>
  <div class="col-md-6">
    <div class="card">
      <div class="card-header" style="background-color: lightsalmon;">
        <h3 class="card-title">MALA <span style="color: red;"> FILLATUNNIDA</span></h3>
      </div>
      <div class="card-body">
        <div class="table-responsive">
          <img src="https://sindunesia.com/wp-content/uploads/2021/01/muslimah-sedang-berbicara-di-telephon.jpg" width="300px" height="180px">
          <h2>Contact</h2><hr>
          <h3>Address:</h3>
          <p v-for="(row, index) in agenda" :key="index">{{ row.address}}</p>
          <h3>Phone:</h3>
          <p v-for="(row, index) in agenda" :key="index">{{ row.phone }}</p>
          <h3>Email:</h3>
          <p v-for="(row, index) in agenda" :key="index"><u>{{ row.email }}</u></p>
          <h2>Languanges</h2><hr>
          <p v-for="(row, index) in agenda" :key="index">{{ row.languanges1 }}</p>
          <p v-for="(row, index) in agenda" :key="index">{{ row.languanges2 }}</p>
          <h2>Hobbies</h2><hr>
          <ul>
          <li><p v-for="(row, index) in agenda" :key="index">{{ row.hobbies1 }}</p></li>
          <li><p v-for="(row, index) in agenda" :key="index">{{ row.hobbies2 }}</p></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: 'AgendaShow',
        computed: {
            agenda() {
                return this.$store.state.listAgenda
            }
        }
    }
</script>

<style scoped>
.card-body {
background-color: powderblue;
height: 935px;
}
</style>