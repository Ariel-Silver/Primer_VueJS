<template>
    <table class="table table-striped table-dark">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Nombre</th>
      <th scope="col">Apellido</th>
      <th scope="col">RUN</th>
      <th scope="col">Nacimiento</th>
      <th scope="col">Edad</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="(Usuario, $index) in Usuarios" :key="$index">
      <td>{{$index}}</td>
      <td>{{Usuario.Nombre}}</td>
      <td>{{Usuario.Apellido}}</td>
      <td>{{Usuario.RUN}}</td>
      <td>{{Usuario.Nacimiento}}</td>
      <td>{{Usuario.Edad}}</td>
    </tr>
  </tbody>
</table>
 
</template>
<script>
export default {
  name: "app",
  data: () => ({
    Usuarios: 
    [{
      Nombre: "Elsa",
      Apellido: "Pallo",
      Run:"11.222.333-4",
      Nacimiento: "10/01/1991",
      Edad: "30"
    },
    {
      Nombre: "Aquiles",
      Apellido: "Baeza",
      Run:"55.666.777-8",
      Nacimiento: "20/04/2001",
      Edad: "20"
    },
     {
      Nombre: "Soila",
      Apellido: "Cerda",
      Run:"99.111.222-3",
      Nacimiento: "10/01/2011",
      Edad: "10"
    }]
  }),
};
</script>

<style>

</style>

