<template>
  <div id="app">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <br />
          <h1>Tabla de Usuarios</h1>
          <br />
          <table class="table table-bordered table-dark">
            <thead>
              <tr>
                <th class="titulo" scope="col">#</th>
                <th class="titulo" scope="col">Nombre</th>
                <th class="titulo" scope="col">Apellido</th>
                <th class="titulo" scope="col">RUN</th>
                <th class="titulo" scope="col">Nacimiento</th>
                <th class="titulo" scope="col">Edad</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <th class="numeral" scope="row">1</th>
                <td class="contenido">{{usuarios[0].nombre}}</td>
                <td class="contenido">{{usuarios[0].apellido}}</td>
                <td class="contenido">{{usuarios[0].run}}</td>
                <td class="contenido">{{usuarios[0].nacimiento}}</td>
                <td class="contenido">{{usuarios[0].edad}}</td>
              </tr>
              <tr>
                <th class="numeral" scope="row">2</th>
                <td class="contenido">{{usuarios[1].nombre}}</td>
                <td class="contenido">{{usuarios[1].apellido}}</td>
                <td class="contenido">{{usuarios[1].run}}</td>
                <td class="contenido">{{usuarios[1].nacimiento}}</td>
                <td class="contenido">{{usuarios[1].edad}}</td>
              </tr>
              <tr>
                <th class="numeral" scope="row">3</th>
                <td class="contenido">{{usuarios[2].nombre}}</td>
                <td class="contenido">{{usuarios[2].apellido}}</td>
                <td class="contenido">{{usuarios[2].run}}</td>
                <td class="contenido">{{usuarios[2].nacimiento}}</td>
                <td class="contenido">{{usuarios[2].edad}}</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
const app = new Vue({
  el: "#app",
  data: {
    usuarios: [
      {
        nombre: "Juan",
        apellido: "Dominguez",
        run: "16.843.377-8",
        nacimiento: "12-01-88",
        edad: 32
      },
      {
        nombre: "Eduardo",
        apellido: "Lara",
        run: "17.943.285-7",
        nacimiento: "30-11-90",
        edad: 29
      },
      {
        nombre: "Camila",
        apellido: "Puelma",
        run: "18.326.389-0",
        nacimiento: "02-12-59",
        edad: 60
      }
    ]
  }
});
</script>

<style>
.container{
  width:  100%;
}

h1 {
  text-align: center;
  color: blue;
  font-family: "Times New Roman", Times, serif;
}

body {
  background-color: yellow;
}

.titulo {
  color: cyan;
  text-align: center;
}

.contenido {
  color: red;
  text-align: center;
}

.numeral {
  color: green;
  text-align: center;
}
</style>
