<div class="carousel-item w-100 text-center active">
    <h3>Mettre à disposition des utilisateurs un service informatique - Stage à l'IBCP</h3>
    <br>
    <p>Présentation des tests de déploiement de l'application</p>
</div>
<div class="carousel-item w-100 text-center">
    <h3>L'application NPSA-NG</h3>
    <br>
    <p>application web codée en FastAPI (python) et Svelte (Javascript)</p>
    <p>projet de 8 semaines pour refaire une vielle application en Perl.</p>
    <p>Elle propose des systèmes de calcul aux bio-informaticiens</p>
    <img src="images/npsa.jpeg" alt="page d'input" style="max-width:700px;">
</div>
<div class="carousel-item w-100 text-center">
    <h3>Environnement de test</h3>
    <br>
    <p>Mise a disposition d'un serveur Debian 12</p>
    <p>clonage du code depuis le GitLab de l'IBCP</p>
    <p>Lancement des applications en mode "host"</p>
    <p><code>fastapi run</code> et <code>npm run dev -- --host</code></p>
</div>
<div class="carousel-item w-100 text-center">
    <h3>Ajout du HTTPS</h3>
    <br>
    <div class="row">
        <div class="col">
            <p>FastAPI : utilisation d'une commande uvicorn pour le lancement</p>
            <img src="images/fastapi-https.png" alt="uvicorn https">
        </div>
        <div class="col">
            <p>Svelte : Changement de la configuration Vite</p>
            <img src="images/svelte-https.png" alt="vite https" style="max-width: 350px;">
        </div>
    </div>
</div>
<div class="carousel-item w-100 text-center">
    <h3>Lancement en daemon du backend</h3>
    <p>ajout d'une configuration Gunicorn</p>
    <img src="images/gunicorn-1.png" alt="gunicorn python">
    <br>
    <img src="images/gunicorn-2.png" alt="gunicorn python">
</div>
<div class="carousel-item w-100 text-center">
    <h3>Build du frontend</h3>
    <p>Utilisation de SvelteKit -> compilation vers un site statique pas possible</p>
    <p>Utilisation d'un adaptateur vite pour la compilation</p>
    <img src="images/adapter-node.png" alt="adaptateur node pour sveltekit">
    <br>
    <p>Lancement via la commande <code>node index.js</code> dans le répertoire de build</p>
</div>