<div class="carousel-item w-100 text-center active">
    <h3>Gestion de patrimoine informatique - OCS Inventory</h3>
    <br>
    <p>présentation du TP, des objectifs et des travaux réalisés</p>
</div>
<div class="carousel-item w-100 text-center">
    <h3>Objectifs</h3>
    <br>
    <p>1. Déployer un OCS inventory sur un serveur debian / ubuntu</p>
    <p>2. Créer et référencer au minimum des machines windows server, macOS, ubuntu et windows 7</p>
    <p>3.1 Effectuer un téldéploiement</p>
    <p>3.2 Installer une extention</p>
    <p>4. Créer une machine GLPI et y importer les appareils référencés par OCS</p>
    <p>5. Installer et configurer Fusion Inventory</p>
</div>
<div class="carousel-item w-100 text-center">
    <h3>Installation d'OCS</h3>
    <br>
    <p>Décision de le faire avec Docker après une installation en dure non fonctionnelle.</p>
    <p>application OCS (port : 7000)</p>
    <p>base MySQL pour OCS</p>
    <p>application GLPI (port : 5000)</p>
    <p>base MariaDB pour GLPI</p>
    <p>application phpLocation (port 8000)</p>
    <p>reverse proxy Nginx</p>
</div>
<div class="carousel-item w-100 text-center">
    <h3>Référencement des machines</h3>
    <br>
    <img src="images/ocs-ws.png" alt="ocs depuis windows server" style="max-width: 750px;">
</div>
<div class="carousel-item w-100 text-center">
    <h3>Localisation des machines</h3>
    <br>
    <p>La localisation se fait arbitrairement à partir des adresses IP</p>
    <img src="images/ocs-location.png" alt="localisation des machines ocs" style="max-width: 750px;">
</div>
<div class="carousel-item w-100 text-center">
    <h3>Ajout d'une Extention</h3>
    <br>
    <img src="images/ocs-extention.png" alt="installation d'une extention" style="max-width: 750px;">
</div>
<div class="carousel-item w-100 text-center">
    <h3>Synchronisation avec GLPI</h3>
    <br>
    <img src="images/ocs-glpi.png" alt="machines sur GLPI" style="max-width: 750px;">
</div>
<div class="carousel-item w-100 text-center">
    <h3>Ce qui n'a pas marché</h3>
    <br>
    <p>Installation de l'agent OCS sur Windows 7</p>
    <p>Installation de l'agent OCS sur MacOS</p>
    <p>L'extention n'apparaissait pas</p>
    <p>Le plugin fusionInvnetory ne fonctionnait pas</p>
    <p>Le télédéploiement reste en attente et rien n'est installé</p>
    <p>La localisation des appareils devait être faite directement sur une page d'OCS (php / perl)</p>
</div>