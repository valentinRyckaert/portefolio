<script>
    import Skills from "../../components/competences/Skills.svelte";
    import Certifications from "../../components/competences/Certifications.svelte";
</script>

<div>
    <div class="row text-center my-5">
        <h2>Mes compétences</h2>
    </div>
    <div class="row text-center fs-5 p-4 border border-5 rounded-5">
        <p>Etant de nature curieuse, j'ai exploré pendant mon parcours des domaines très diverses. Développeur, je suis pourtant attiré par l'administration système, le réseautage, le DevOps, et bien d'autres choses.</p>
        <p>Ainsi, en ce qui concèrne le développement, je m'intéresse tout autant au développement web que mobile ou logiciel.</p>
    </div>
    <div class="row text-center my-5">
        <Skills/>
    </div>
    <div class="row text-center my-5">
        <h2>Mes Certifications</h2>
    </div>
    <div class="row text-center my-5">
        <Certifications/>
    </div>
</div>