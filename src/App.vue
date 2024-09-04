<template>
    <div class="container">

      <headerComponent />

      <h1 class="titulo">Manager Project</h1>
        <div>
          <groupsComponent/>
        </div>

          <div class="projects">
            <div>
            </div>
          </div>

        <footer>
          <b>Copyright © 2019 </b>
          <a href="#">. Contact Point 360</a>
          <p>. All rights reserved.</p>
        </footer>

    </div>
</template>

<script>
import groupsComponent from './components/groupsComponent.vue';
import headerComponent from './components/headerComponent.vue'

export default {
  name: 'App',
  components: {
    headerComponent,
    groupsComponent,
  }
}
</script>

<style scoped>


.container {
  display: flex;
  flex-direction: column;
  min-width: 90vw;
  min-height: 100vh;
  background-color: #dae1e7;
}

.titulo {
  font-family: "Anton SC", sans-serif;
  font-weight: 400;
  font-style: normal;
  color: #06164D;
  margin: 15px 0 0 25px;
}

/*=================footer=================*/

footer {
  margin-top: auto;
  padding: 20px ;
  max-width: 100vw;
  background-color: white;
  border-top: 1px solid rgb(187, 187, 187);
  border-bottom: 1px solid rgb(187, 187, 187);
  font-family: "Blinker", sans-serif;
}

footer a {
  text-decoration: none;
  font-weight: bold;
  color: #06164D;
}

footer p  {
  color: rgb(141, 141, 141);
  display: inline;
}

footer b {
  color: rgb(141, 141, 141);
}

/*==================================*/

</style>
