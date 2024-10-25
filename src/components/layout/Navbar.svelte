<script>
  import { onMount } from 'svelte';
  
  export let active;

  onMount(()=>{
    setActiveRoute('/');
  });

  function setActiveRoute(route) {
    active = route;
  }
</script>

<nav class="navbar navbar-expand-lg bg-body-transparent">
    <div class="container-fluid">
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-center" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item mx-3">
            <a class="nav-link {active == '/' ? "active" : ""}" aria-current="page" href="/portefolio" on:click={event => setActiveRoute('/')}>Accueil</a>
          </li>
          <li class="nav-item mx-3">
            <a class="nav-link {active == '/formation' ? "active" : ""}" href="/formation" on:click={event => setActiveRoute('/formation')}>Formation</a>
          </li>
          <li class="nav-item mx-3">
            <a class="nav-link {active == '/experience' ? "active" : ""}" href="/experience" on:click={event => setActiveRoute('/experience')}>Expérience</a>
          </li>
          <li class="nav-item mx-3">
            <a class="nav-link {active == '/competences' ? "active" : ""}" href="/competences" on:click={event => setActiveRoute('/competences')}>Compétences</a>
          </li>
          <li class="nav-item mx-3">
            <a class="nav-link {active == '/projets' ? "active" : ""}" href="/projets" on:click={event => setActiveRoute('/projets')}>Projets</a>
          </li>
          <li class="nav-item mx-3">
            <a class="nav-link {active == '/a_propos' ? "active" : ""}" href="/a_propos" on:click={event => setActiveRoute('/a_propos')}>A propos de ce site</a>
          </li>
        </ul>
      </div>
    </div>
</nav>