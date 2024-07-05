<script>
    import AcordionQuestion from "../components/main/Acordion-question.svelte";
</script>

<div>
    <div class="row p-md-5 px-2 py-5 mb-5 border border-5 rounded-5">
        <div class="col-7">
            <h1 class="text-center mb-5">Bienvenue sur mon Porte-Folio</h1>
            <h5 class="m-3">Je m'appelle Valentin Ryckaert, étudiant en BTS SIO option développement à l'Institution des Chartreux à Lyon.</h5>
            <h5 class="m-3">Je suis curieux, studieux et loyal. Je sais travailler seul comme au sein d'une équipe.</h5>
            <h5 class="m-3">Je suis à l'aise avec les framworks Node.js (Express, Angular, Svelte...), ainsi qu'avec les langages Python, Ruby et Java.</h5>
        </div>
        <div class="col-5">
            <img src="/profil.jpg" class="img-fluid" alt="mon chat">
        </div>
    </div>
    <div class="row p-md-5 px-2 py-5 mb-5 border border-5 rounded-5">
        <AcordionQuestion/>
    </div>    
</div>