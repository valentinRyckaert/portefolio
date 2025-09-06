<div class="carousel-item w-100 text-center active">
    <h3>Gestion de patrimoine informatique - PCA-PRA</h3>
    <br>
    <p>présentation du TP, des objectifs et des travaux réalisés</p>
</div>
<div class="carousel-item w-100 text-center">
    <h3>Contexte</h3>
    <br>
    <p>Chaque groupe construit une architecture. Cette architecture va être attaqué par un autre groupe d'une manière définie.</p>
    <p>On ne sait à l'avance ni quand ni comment on va être attaqué.</p>
</div>
<div class="carousel-item w-100 text-center">
    <h3>Notre architecture</h3>
    <br>
    <div class="row">
        <div class="col">
            <h5>BATIMENT A :</h5>
            <p>client windows 11</p>
            <p>AD windows server</p>
        </div>
        <div class="col">
            <h5>BATIMENT B :</h5>
            <p>client windows 11</p>
            <p>RODC de l'AD</p>
            <p>serveur web Fedora Server hébergeant une stack docker WordPress / MariaDB</p>
        </div>
    </div>
    <br>
    <p>Roles dans l'entreprise : 1 développeur (Valentin), 2 administrateurs systèmes (Lucas, Louis)</p>
</div>
<div class="carousel-item w-100 text-center">
    <h3>Mise en place de PCA et PRA</h3>
    <br>
    <img src="images/pca-pra.png" alt="exemple pca-pra">
</div>
<div class="carousel-item w-100 text-center">
    <h3>Etat des lieux du dimanche 16 février</h3>
    <br>
    <p>10h00 : l'état des lieux est effectué, rien d'anormal remarqué</p>
    <p>11H50 : nouvel état des lieux avec l'administrateur systèmes (Louis) pour un problème de connection au WordPress</p>
    <p>12H15 : le développeur remarque l'impossibilité de se connecter aux deux machines clientes windows 11, les mots de passe ont été modifiés. Déclanchement du PRA pour l'impossibilité de connection aux sessions windows.</p>
    <p>12H20 : L'administrateur systèmes (Louis) se connecte à l'AD avec le compte administrateur, qui n'a pas été modifié. Il restaure un à un les mots de passe des utilisateurs.</p>
    <p>Le deuxième administrateur n'étant pas joignable, c'est le développeur qui se charge de vérifier dans le même temps le bon fonctionnement de chaque compte.</p>
    <p>12H45 : Tous les utilisateurs sont de nouveau utilisables</p>
    <p>13H00 : rédaction de ce compte rendu terminée.</p>
</div>
<div class="carousel-item w-100 text-center">
    <h3>Analyse et solutions trouvées</h3>
    <br>
    <p>Le problème n'a pas été remarqué lors des états des lieux du samedi et du dimanche matin : contrôles effectués par les administrateurs</p>
    <p>L'un des administrateurs systèmes n'était pas joignable : le développeur peut le remplacer (ajouter au PRA)</p>
    <p>Oubli de déconnecter l'AD du réseau : penser à le faire à l'avenir</p>
    <p>Restauration des mots de passe et de leur vérification simultanée : à ajouter au PRA (gain de temps)</p>
</div>