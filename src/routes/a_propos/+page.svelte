<script>
    import TitleTextImage from "../../components/TitleTextImage.svelte";
</script>

<div class="row mb-5">
    <h2 class="text-center">A propos de ce site</h2>
</div>
<div class="row">
    <TitleTextImage imageLink="/svelte.svg" alt="Logo Svelte" imagePos="right" titlePos="start">
        <span slot="title">
            Ce site est fait avec Svelte et Bootstrap
        </span>
        <span slot="body">
            <p>
                Bootstrap est un framework CSS qui met à disposition des paramettres css simplifiant l'élaboration du Design d'un site web.
                En plus d'être simple d'utilisation, Bootstrap offre la possibilité de modifier le thème générique, ce qui offre une marge de customisation importante.
            </p>
            <p>
                Svelte est un compilateur Javascript (<i>de facto</i> considéré comme un framework frontend) permettant de créer des applications web et des pages web réactives rapidement.
                Il est plus rapide que ses concurrents, car il s'agit d'un compilateur (et n'intéragit donc pas avec le DOM HTML),
                et il est possède une architecture simple, ce qui permet de développer plus efficacement.
            </p>
            <a class="btn btn-link" href="https://svelte.dev/">Le site de Svelte</a>
            <a class="btn btn-link" href="https://getbootstrap.com/">Le site de Bootstrap</a>
        </span>
    </TitleTextImage>
</div>
<div class="row">
    <TitleTextImage imageLink="/opendyslexic.png" alt="Logo OpenDyslexic" imagePos="left" titlePos="end">
        <span slot="title">
            La police de ce site est adaptée aux dyslexiques
        </span>
        <span slot="body">
            <p>
                OpenDyslexic est un projet open-source visant à concevoir une police peremettant de contrer certains symptômes de la dyslexie.
                Elle est le résultat d'un travail commun entre des designers et des études scientifiques sur la dyslexie.
            </p>
            <p>
                Je suis légèrement dyslexique, et cette police me permet de diminuer grandement mes effort pour lire.
                Je l'utilise par défaut sur mon ordinateur.
            </p>
            <a class="btn btn-link" href="https://opendyslexic.org/">Le site OpenDyslexic</a>
        </span>
    </TitleTextImage>
</div>