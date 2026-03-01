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
                    <button class="btn btn-lg btn-primary m-2">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-file-check-fill align-baseline" viewBox="0 0 16 16">
                            <path d="M12 0H4a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h8a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2m-1.146 6.854-3 3a.5.5 0 0 1-.708 0l-1.5-1.5a.5.5 0 1 1 .708-.708L7.5 8.793l2.646-2.647a.5.5 0 0 1 .708.708"/>
                        </svg>
                        Mon CV
                    </button>
                </a>
                <a href="https://github.com/valentinRyckaert" target="_blank">
                    <button class="btn btn-lg btn-primary m-2">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-github align-baseline" viewBox="0 0 16 16">
                            <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27s1.36.09 2 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.01 8.01 0 0 0 16 8c0-4.42-3.58-8-8-8"/>
                        </svg>
                        Mon Github
                    </button>
                </a>
                <a href="https://www.linkedin.com/in/valentin-ryckaert-29b3052a2/" target="_blank">
                    <button class="btn btn-lg btn-primary m-2">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-linkedin align-baseline" viewBox="0 0 16 16">
                            <path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854zm4.943 12.248V6.169H2.542v7.225zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248S2.4 3.226 2.4 3.934c0 .694.521 1.248 1.327 1.248zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016l.016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225z"/>
                        </svg>
                        Mon Linkedin
                    </button>
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
    