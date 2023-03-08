<template>
    <div>
      <h1>Liste des élèves</h1>
      <table class="table">
        <thead>
          <tr>
            <th>Nom</th>
            <th>Prénom</th>
            <th>Age</th>
            <th>Classe</th>
            <th>Actions</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="eleve in eleve" :key="eleve.id">
            <td>{{ eleve.user.name }}</td>
            <td>{{ eleve.user.prename }}</td>
            <td>{{ eleve.user.age }}</td>
            <td>{{ eleve.classe.name }}</td>
            <td> <router-link :to="{ name: 'EleveDetails', params: { id: eleve.id } }" class="btn btn-primary">Détails</td>
          </tr>
          </tbody>
          </table>
          </div>
</template>