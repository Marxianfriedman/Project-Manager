<template>
    <div class="container">
      <button>Development</button>
        <div class="container2">
          <h2 class="titulo">Lista de proyectos</h2>
                <projectCreate/>
        </div>
    </div>
</template>

<script>

import projectCreate from './projectCreate.vue';

export default {
    name: "projectListComponent",
    components: {
      projectCreate
    }
}

</script>

<style scoped>

.container {
  display: flex;
  flex-direction: column;
  background-color: #f5f7f9;
}


button {
  background-color: #2e197b;
  color: white;
  padding: 1rem; 
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 17px;
  width: 150px;
}


button:hover {
  background-color: #281764;;
}

.titulo {
  font-size: 30px;
  font-family: "Marcellus SC", serif;
  margin: 0 0 10px 0;
}

.container2 {
  font-family: "Blinker", sans-serif;
  border: 0.1px solid rgb(225, 222, 222);
  border-radius: 5px;
  padding:  1rem;
  box-shadow: 0.2px 1px 2px 0px rgb(190, 190, 190);
  background-color: white;
  margin: 10px;
}

</style>