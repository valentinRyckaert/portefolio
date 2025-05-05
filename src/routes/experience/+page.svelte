<script>
    import TitleTextImage from "../../components/TitleTextImage.svelte";
</script>

<div class="row mb-5">
    <h2 class="text-center">Mon expérience</h2>
</div>
<div class="row">
    <TitleTextImage imageLink="images/logo-ibcp.png" alt="Logo IBCP" imagePos="left" titlePos="start">
        <span slot="title">
            Stage à l'Institut de Biologie et Chimie des Protéines (IBCP) - mars-avril 2025
        </span>
        <span slot="body">
            <p>Stage de 8 semaines en développement Web.</p>
            <p>Développement de l'application NPSA-NG intégrant des systèmes de calcul de protéines (Clustal Omega, Blastp, Alphafold 3...).</p>
            <p>Utilisation des Frameworks FastAPI (python) et Svelte (JavaScript).</p>
            <p>rédaction d'un rapport de stage.</p>
        </span>
    </TitleTextImage>
    <TitleTextImage imageLink="images/xev.png" alt="Logo Xev" imagePos="right" titlePos="end">
        <span slot="title">
            Stage au sein de l'entreprise Xev - juin-juillet 2024
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
    <TitleTextImage imageLink="images/iap.jpg" alt="Logo IAP" imagePos="left" titlePos="start">
        <span slot="title">
            Stage à l'Institut d'Astrophysique de Paris - octobre 2021
        </span>
        <span slot="body">
            <p>Stage d'une semaine.</p>
            <p>J'ai assisté à des conférences sur de nombreux sujets (exoplanètes, système solaire, cosmologie, ondes gravitationnelles...).</p>
            <p>Visite des ateliers de fabrication de téléscopes.</p>
        </span>
    </TitleTextImage>
    <TitleTextImage imageLink="images/inria.png" alt="Logo Inria" imagePos="right" titlePos="end">
        <span slot="title">
            Stage à l'Institut National de Recherche en Informatique et Automatique (INRIA) - juin 2021
        </span>
        <span slot="body">
            <p>Stage d'observation d'une semaine au centre Inria de Lyon.</p>
            <p>Découverte de l'intrication quantique et de l'informatique théorique à l'aide de problèmes mathématiques.</p>
            <p>Découverte de l'environnement de la recherche scientifique.</p>
            <p>rédaction d'un rapport de stage.</p>
        </span>
    </TitleTextImage>
</div>
