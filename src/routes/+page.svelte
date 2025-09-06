<script>
    import AcordionQuestion from "../components/main/Acordion-question.svelte";
</script>

<div>
    <div class="row p-lg-5 px-2 py-5 mb-5 border border-5 rounded-5">
        <div class="cust-col-lg-7">
            <h1 class="text-center mb-5">Bienvenue sur mon Porte-Folio</h1>
            <h5 class="text-center mx-3 my-4">Je m'appelle Valentin Ryckaert, étudiant en Informatique et CyberSécurité (ICS) à l'école d'ingénieur CPE Lyon.</h5>
            <h5 class="text-center mx-3 my-4">Je suis diplômé du BTS SIO option développement à l'Institution des Chartreux à Lyon.</h5>
            <h5 class="text-center mx-3 my-4">Curieux, studieux et loyal, je sais travailler seul comme au sein d'une équipe.</h5>
            <h5 class="text-center mx-3 my-4">J'utilise différentes technologies web (Vue.js, FastAPI, Svelte...) ainsi que les langages Python, Java, Typescript et Ruby.</h5>
            <div class="text-center pt-4 my-4">
                <a href="docs/CV-Valentin-Ryckaert.pdf" target="_blank">
                    <button class="btn btn-lg btn-primary m-2">Mon CV</button>
                </a>
            </div>
        </div>
        <div class="cust-col-lg-5">
            <img src="images/profil.jpg" class="img-fluid mx-auto" alt="profil">
        </div>
    </div>
    <div class="row p-md-5 px-2 py-5 mb-5 border border-5 rounded-5">
        <AcordionQuestion/>
    </div>    
</div>

<style>
    img {
      max-width: 320px;
      display: block;
      margin-left: auto;
      margin-right: auto;
    }
    @media (min-width: 1110px) {
        .cust-col-lg-5 {
            flex: 0 0 auto;
            width: 41.66666667%;
        }
        .cust-col-lg-7 {
            flex: 0 0 auto;
            width: 58.33333333%;
        }
    }
</style>
    