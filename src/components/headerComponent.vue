<template>
    <div>
      <header>
        <div class="izquierda">
          <img class="menu" :src="require('./img/menu.png')" alt="">
        </div>
        <div class="derecha">
          <div class="notificaciones">
            <img class="campana" :src="require('./img/campana.png')" alt="notificaciones">
            <div class="numero">0</div>
          </div>
          <div class="img-perfil">
            <img class="img-perfil1" :src="require('./img/usuario.png')" alt="img-perfil">
          </div>
          <div class="nombre-usuario">Nombre de Usuario</div>
        </div>
      </header>
    </div>
  </template>
  
  <script>
  export default {
    name: 'headerComponent'
  }
  </script>

<style scoped>
header {
  height: 55px;
  display: flex;
  justify-content: space-between;
  background-color: white;
}

.izquierda {
  width: 55px;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}

.menu{
  width: 30%;
  height: 30%;
}

.derecha {
  width: 265px;
  height: 100%;
  display: flex;
}

.notificaciones {
  height: 100%;
  width: 55px;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}


.numero {
  background-color: yellow;
  font-size: 11px;
  padding: 5px;
  margin-bottom: 18px;
  margin-right: 20px;
}

.campana {
  width: 50%;
  height: 50%;
  margin-left: 10px;
}

.img-perfil {
  height: 100%;
  width: 55px;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}

.img-perfil1 {
  height: 65%;
  width: 65%;
  box-shadow: 1px 3px 5px 1.5px rgb(158, 156, 156);
  border-radius: 100%;
}

.nombre-usuario {
  height: 100%;
  width: 155px;
  display: flex;
  justify-content: start;
  align-items: center;
  font-family: "Blinker", sans-serif;
  color: rgb(141, 141, 141);
  cursor: pointer;
}

.nombre-usuario:hover {
  color: rgb(98, 98, 98);
}
</style>