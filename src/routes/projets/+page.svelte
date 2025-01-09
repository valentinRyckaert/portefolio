<script>
    import Projet from "../../components/projets/Projet.svelte";
</script>

<div class="row mb-5">
    <h2 class="text-center">Mes projets</h2>
</div>
<div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-4">
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
        <Projet listTools="{['Docker','MkDocs','Markdown']}" imageLink="images/mkdocs.png" imageAlt="Logo MkDocs">
            <span slot="title">
                Documentation Web
            </span>
            <span slot="text">
                Développement d'une Documentation web en markdown avec MkDocs.
                Travail par deux.
            </span>
        </Projet>
    </div>
    <div class="col">
        <Projet listTools="{['PHP','composer']}" linkTo="https://github.com/valentinRyckaert/Piment" imageLink="images/piment.png" imageAlt="Logo piment">
            <span slot="title">
                Application Piment
            </span>
            <span slot="text">
                Développement d'une Apllication web en PHP natif
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
</div>