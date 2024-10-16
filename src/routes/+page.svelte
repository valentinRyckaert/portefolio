<script>
    import AcordionQuestion from "../components/main/Acordion-question.svelte";
</script>

<div>
    <div class="row p-lg-5 px-2 py-5 mb-5 border border-5 rounded-5">
        <div class="cust-col-lg-7">
            <h1 class="text-center mb-5">Bienvenue sur mon Porte-Folio</h1>
            <h5 class="m-3 ">Je m'appelle Valentin Ryckaert, étudiant en BTS SIO option développement à l'Institution des Chartreux à Lyon.</h5>
            <h5 class="m-3">Je suis curieux, studieux et loyal. Je sais travailler seul comme au sein d'une équipe.</h5>
            <h5 class="m-3">Je suis à l'aise avec les technologies web (Django, Svelte, Angular...), ainsi qu'avec les langages Python, Ruby et Java.</h5>
            <div class="text-center pt-4">
                <a href="docs/CV-Valentin-Ryckaert.pdf" download>
                    <button class="btn btn-lg btn-primary mb-4">Mon CV</button>
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
      max-width: 400px;
      display: block;
      margin-left: auto;
      margin-right: auto;
    }
    @media (min-width: 1210px) {
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
    