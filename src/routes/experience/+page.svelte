<script>
    import TitleTextImage from "../../components/TitleTextImage.svelte";
</script>

<div class="row mb-5">
    <h2 class="text-center">Mon expérience</h2>
</div>
<div class="row">
    <TitleTextImage imageLink="images/inria.png" alt="Logo Inria" imagePos="left" titlePos="start">
        <span slot="title">
            Stage à l'Institut National de Recherche en Informatique et Automatique (INRIA)
        </span>
        <span slot="body">
            <p>Stage d'observation d'une semaine au centre Inria de Lyon.</p>
            <p>Découverte de l'intrication quantique et de l'informatique théorique à l'aide de problèmes mathématiques.</p>
            <p>Découverte de l'environnement de la recherche scientifique.</p>
            <p>rédaction d'un rapport de stage.</p>
        </span>
    </TitleTextImage>
    <TitleTextImage imageLink="images/iap.jpg" alt="Logo IAP" imagePos="right" titlePos="end">
        <span slot="title">
            Stage à l'Institut d'Astrophysique de Paris
        </span>
        <span slot="body">
            <p>Stage d'une semaine.</p>
            <p>J'ai assisté à des conférences sur de nombreux sujets (exoplanètes, système solaire, cosmologie, ondes gravitationnelles...).</p>
            <p>Visite des ateliers de fabrication de téléscopes.</p>
        </span>
    </TitleTextImage>
    <TitleTextImage imageLink="images/xev.png" alt="Logo Xev" imagePos="left" titlePos="start">
        <span slot="title">
            Stage au sein de l'entreprise Xev
        </span>
        <span slot="body">
            <p>Stage de 6 semaines en développement Web chez Xev.</p>
            <p>Expérimentation des méthodologies agiles (Jira)</p>
            <p>Utilisation des outils gcloudCLI, PostgreSQL, Strapi, Angular et Firestore.</p>
            <p>Analyse de données via des scripts Python.</p>
            <p>rédaction d'un rapport de stage.</p>
            <p>Soutenance de stage.</p>
        </span>
    </TitleTextImage>
</div>
