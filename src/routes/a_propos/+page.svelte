<script>
    import TitleTextImage from "../../components/TitleTextImage.svelte";
</script>

<div class="row mb-5">
    <h2 class="text-center">A propos de ce site</h2>
</div>
<div class="row">
    <TitleTextImage imageLink="/sveltebootstrap.png" alt="Logo Svelte et Bootstrap" imagePos="right" titlePos="start">
        <span slot="title">
            Ce site est fait avec Svelte et Bootstrap
        </span>
        <span slot="body">
            <p>
                Bootstrap est un framework CSS qui met à disposition des paramettres css simplifiant l'élaboration du Design d'un site web.
            </p>
            <p>
                Je ne suis pas un grand fan de Boostrap, notamment parce que j'apprécie manipuler du css/scss vania (sans framework/librairie).
                Malgré cela, je dois avouer que Bootstrap, en plus d'être efficace et particulièrement simple d'utilisation, possède une marge de customisation très importante, ce qui permet de s'éloigner rapidement du thème générique.
                C'est pour cette raison que j'ai tendance à l'utiliser pour mes projets personnels.
            </p>
            <p>
                Svelte est un compilateur Javascript (<i>de facto</i> considéré comme un framework frontend) permettant de créer des applications web et des pages web réactives rapidement.
            </p>
            <p>
                Svelte, quant à lui, à deux avantages par rapport à ses concurrents.
                il est rapide, car il s'agit d'un compilateur (et n'intéragit donc pas avec le DOM HTML),
                et il est possède une architecture simple, ce qui permet de développer rapidement.
            </p>
        </span>
    </TitleTextImage>
</div>