<script>
    import Projet from "../../components/projets/Projet.svelte";
</script>

<div class="row mb-5">
    <h2 class="text-center">Mes projets</h2>
</div>
<div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-4">
    <div class="col">
        <Projet listTools="{['React', 'CSS', 'Bootstrap']}" linkTo="https://github.com/killex8569/DonnezNousUnStageOuUneAlternance" imageLink="" imageAlt="">
            <span slot="title">
                Donnez Nous un Stage ou une Alternance
            </span>
            <span slot="text">
                Porte-folio en React fait dans le cadre de nos recherches pour le BAC+4 en alternance
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['Markdown']}" imageLink="" imageAlt="">
            <span slot="title">
                Europeanize Yourself!
            </span>
            <span slot="text">
                Document listant les alternatives numériques européennes aux outils américains et asiatiques
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['Typer (Python)', 'NVD CVE', 'NMAP']}" linkTo="https://github.com/SpeeDelta/CVE-Searcher" imageLink="" imageAlt="">
            <span slot="title">
                CVEsearcher
            </span>
            <span slot="text">
                Outil de scan réseau permettant de lister les CVE accessibles
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['Python', 'C', 'Bash']}" linkTo="https://github.com/killex8569/algo-en-27-exos" imageLink="" imageAlt="">
            <span slot="title">
                L'algo en 27 exos
            </span>
            <span slot="text">
                Exercices progressifs pour apprendre l'algorithmie
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['FastAPI','Svelte','MariaDB','Apache']}" linkTo="https://github.com/valentinRyckaert/ITAM-backend" imageLink="" imageAlt="">
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
        <Projet listTools="{['PHP','composer']}" linkTo="https://github.com/valentinRyckaert/Piment">
            <span slot="title">
                Application Piment
            </span>
            <span slot="text">
                Développement d'une Application web en PHP natif
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['C']}" linkTo="https://github.com/valentinRyckaert/ALL">
            <span slot="title">
                Assembly-Like Language (ALL)
            </span>
            <span slot="text">
                Langage de programmation inspiré de la syntaxe des langages assembleurs
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['Docker','WordPress', 'WooCommerce', 'Hubspot', 'Yoast SEO']}">
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
        <Projet listTools="{['Laravel','Tailwind','Tuleap','Figma']}">
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
        <Projet listTools="{['Django','Bootstrap','SQLite']}" imageAlt="">
            <span slot="title">
                MonContrat
            </span>
            <span slot="text">
                Application web de type CRUD : formulaire générant un contrat et stockage des différents contrats.
            </span>
        </Projet>
    </div>
</div>