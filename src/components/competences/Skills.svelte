<script>
  import UnSkill from "./UnSkill.svelte";

  let skillFamilyList = [
    "Web",
    "Programmation",
    "Base de données",
    "Système/Réseau",
    "Cybersécurité",
    "DevOps",
    "DPL/Webmarketing",
    "Soft Skills",
    "Langues",
  ];

  let skillsDictionnary = [
    // Web
    {
      "Angular": 'images/angular.png',
      "Svelte": 'images/svelte.svg',
      "Express": 'images/nodejs.png',
      "Bootstrap": 'images/bootstrap.png',
      "Figma": 'images/figma.png',
      "SASS": 'images/sass.png',
    },
    // Programmation
    {
      "Python": 'images/python.png',
      "Ruby": 'images/ruby.png',
      "Java": 'images/java.png',
      "C#": 'images/c_sharp.png',
      "TypeScript": 'images/typescript.png',
      "Go": 'images/go.png',
    },
    // Base de Données
    {
      "MySQL": 'images/mysql.png',
      "PostgreSQL": 'images/postgresql.png',
      "MongoDB": 'images/mongodb.png',
      "Firestore": 'images/firestore.png',
    },
    // Système/Réseau
    {
      "Windows": 'images/windows.png',
      "Linux": 'images/linux.png',
      "Serveur Linux": 'images/debian.png',
      "DNS": '',
      "Routage": '',
    },
    // Cybersécurité
    {
      "Certificat": '',
      "Horodatage": '',
      "Chiffrement": '',
      "P2P": '',
    },
    // DevOps
    {
      "Docker": 'images/docker.png',
      "Github": 'images/github.png',
      "Gitlab": 'images/gitlab.png',
      "Microsoft Azure": 'images/azure.png',
    },
    // DPL/Webmarketing
    {
      "WordPress": 'images/wordpress.png',
      "Référencement": '',
      "E-mailing": '',
    },
    // Soft Skills
    {
      "Autoapprenissage": '',
      "Travail en équipe": '',
      "Conduite de projet": '',
    },
    // Langues
    {
      "Anglais": '',
      "Allemand": '',
    },
  ];


  let active = skillFamilyList[0];
</script>

<div class="card">
    <div class="card-header">
      <ul class="nav nav-tabs card-header-tabs justify-content-center">
        {#each skillFamilyList as skillName}
          <li class="nav-item">
            <button class="nav-link {active == skillName ? "active" : ""}" on:click={() => active = skillName}>{skillName}</button>
          </li>
        {/each}
      </ul>
    </div>
    <div class="card-body">
      <h5 class="mt-2 mb-4">{active}</h5>
        {#if active == skillFamilyList[0]}
          <UnSkill skills={skillsDictionnary[0]}/>
        {:else if active == skillFamilyList[1]}
          <UnSkill skills={skillsDictionnary[1]}/>
        {:else if active == skillFamilyList[2]}
          <UnSkill skills={skillsDictionnary[2]}/>
        {:else if active == skillFamilyList[3]}
          <UnSkill skills={skillsDictionnary[3]}/>
        {:else if active == skillFamilyList[4]}
          <UnSkill skills={skillsDictionnary[4]}/>
		    {:else if active == skillFamilyList[5]}
          <UnSkill skills={skillsDictionnary[5]}/>
		    {:else if active == skillFamilyList[6]}
          <UnSkill skills={skillsDictionnary[6]}/>
	    	{:else if active == skillFamilyList[7]}
          <UnSkill skills={skillsDictionnary[7]}/>
	    	{:else if active == skillFamilyList[8]}
          <UnSkill skills={skillsDictionnary[8]}/>
		    {:else if active == skillFamilyList[9]}
          <UnSkill skills={skillsDictionnary[9]}/>
		    {:else if active == skillFamilyList[10]}
          <UnSkill skills={skillsDictionnary[10]}/>
        {/if}
    </div>
</div>
