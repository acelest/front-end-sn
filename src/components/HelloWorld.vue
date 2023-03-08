<template>

  <div class="container mt-5">
  <div class="row justify-content-center">
    <div class="col-md-6">
      <h1 class="text-center mb-4">Ajouter un élève</h1>
      <form id="add-student-form">
        
        <div class="form-group">
          <label for="student-name">Nom</label>
          <input type="text" class="form-control" id="student-name" name="name" required>
        </div>
        <div class="form-group">
          <label for="student-prename">Prénom</label>
          <input type="text" class="form-control" id="student-prename" name="prename" required>
        </div>
        <div class="form-group">
          <label for="student-age">Age</label>
          <input type="number" class="form-control" id="student-age" name="age" required>
        </div>
        <div class="form-group">
          <label for="student-gender">Genre</label>
          <select class="form-control" id="student-gender" name="gender" required>
            <option value="">Sélectionnez le genre</option>
            <option value="0">Femme</option>
            <option value="1">Homme</option>
          </select>
        </div>
        <div class="form-group">
          <label for="student-matricule">Matricule</label>
          <input type="text" class="form-control" id="student-matricule" name="matricule" required>
        </div>
        <div class="form-group">
          <label for="student-class">Classe</label>
          <select class="form-control" id="student-class" name="class" required>
            <option value="">Sélectionnez la classe</option>
            <!-- Les classes peuvent être récupérées via l'API /classes -->
          </select>
        </div>
        <div class="form-group">
          <label for="student-parent">Parent</label>
          <select class="form-control" id="student-parent" name="parent" required>
            <option value="">Sélectionnez le parent</option>
            <!-- Les parents peuvent être récupérés via l'API /parents -->
          </select>
        </div> <br>
        <button type="submit" class="btn btn-primary">Ajouter</button>
      </form>
    </div>
  </div>
</div>
</template>