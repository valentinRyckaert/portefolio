<script>
    import Projet from "../../components/projets/Projet.svelte";
</script>

<div class="row mb-5">
    <h2 class="text-center">Mes projets</h2>
</div>
<div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-4">
    <div class="col">
        <Projet listTools="{['FastAPI','Svelte','MariaDB','Apache']}" linkTo="https://github.com/valentinRyckaert/ITAM-frontend" imageLink="" imageAlt="">
            <span slot="title">
                IT Assets Manager (ITAM)
            </span>
            <span slot="text">
                Développement d'une Application web FastAPI - Svelte, pour la gestion d'inventaire d'actifs informatiques
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['React Native','SupaBase']}" linkTo="https://github.com/valentinRyckaert/Distribute" imageLink="" imageAlt="">
            <span slot="title">
                Distribute
            </span>
            <span slot="text">
                Développement d'une Application mobile React Native : blog permettant aux utilisateurs de partager leurs problèmes informatiques pour éviter de toujours passer par l'assistance informatique
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['PHP','composer']}" linkTo="https://github.com/valentinRyckaert/Piment" imageLink="images/piment.png" imageAlt="Logo piment">
            <span slot="title">
                Application Piment
            </span>
            <span slot="text">
                Développement d'une Application web en PHP natif
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['C']}" linkTo="https://github.com/valentinRyckaert/ALL" imageLink="images/ALL.png" imageAlt="program ALL">
            <span slot="title">
                Assembly-Like Language (ALL)
            </span>
            <span slot="text">
                Langage de programmation inspiré de la syntaxe des langages assembleurs
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['Docker','WordPress', 'WooCommerce', 'Hubspot', 'Yoast SEO']}" imageLink="images/logo_votregouvernement.png" imageAlt="logo VotreGouvernement">
            <span slot="title">
                Site vitrine WordPress
            </span>
            <span slot="text">
                Développement de Présence en Ligne via la création d'un site vitrine.
                Produits vendus non-commerciaux et non-concurrenciels.
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['Laravel','Tailwind','Tuleap','Figma']}" imageLink="images/logoPrixy.png" imageAlt="Logo Prixy">
            <span slot="title">
                Application web de réservation
            </span>
            <span slot="text">
                Développement d'une application web pour l'entreprise fictive Prixy.
                Travail par équipes de cinq. Gestion de projet.
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['GLPI']}" imageLink="images/GLPI.png" imageAlt="Logo GLPI">
            <span slot="title">
                TP GLPI
            </span>
            <span slot="text">
                Mise en place d'un GLPI pour la gestion d'incidents
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['Docker','GLPI','OCS Inventory','Apache','MySQL']}" imageLink="images/OCSInventory.png" imageAlt="Logo GLPI">
            <span slot="title">
                TP OCS
            </span>
            <span slot="text">
                Mise en place d'un OCS Inventory couplé à un GLPI pour la gestion de patrimoine informatique
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['Django','Bootstrap','SQLite']}" linkTo="https://github.com/valentinRyckaert/MonContrat" imageLink="images/moncontrat.png" imageAlt="site de moncontrat">
            <span slot="title">
                Générateur de contrat de partenariat commercial
            </span>
            <span slot="text">
                Application web de type CRUD : formulaire générant un contrat et stockage des différents contrats.
            </span>
        </Projet>
    </div>
</div>