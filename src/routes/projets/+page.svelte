<script>
    import Card from "../../components/projets/Card.svelte";
</script>

<div class="row mb-5">
    <h2 class="text-center">Mes projets</h2>
</div>
<div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-4">
    <div class="col">
        <Card listTools="{['Django','Bootstrap','SQLite']}" imageLink="/eglise.jpg" imageAlt="eglise" linkTo="#">
            <span slot="title">
                Générateur de contrat de partenariat commercial
            </span>
            <span slot="text">
                Application web de type CRUD : formulaire générant un contrat et stockage des différents contrats.
            </span>
        </Card>
    </div>
    <div class="col">
        <Card listTools="{['WordPress', 'WooCommerce', 'Hubspot', 'Yoast SEO']}" imageLink="/logo_votregouvernement.png" imageAlt="logo VotreGouvernement" linkTo="#">
            <span slot="title">
                VotreGouvernement
            </span>
            <span slot="text">
                Développement de Présence en Ligne via la création d'un site vitrine.
                Produits vendus non-commerciaux et non-concurrenciels.
            </span>
        </Card>
    </div>
    <div class="col">
        <Card listTools="{['Laravel','Tailwind','Tuleap','Figma']}" imageLink="/logoPrixy.png" imageAlt="Logo Prixy" linkTo="#">
            <span slot="title">
                Application web de réservation
            </span>
            <span slot="text">
                Développement d'une application web pour l'entreprise fictive Prixy.
                Travail par équipes de cinq. Gestion de projet.
            </span>
        </Card>
    </div>
</div>