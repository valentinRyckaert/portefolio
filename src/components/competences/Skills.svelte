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
      "Angular": '/angular.png',
      "Svelte": '/svelte.svg',
      "Express": '/nodejs.png',
      "Bootstrap": '/bootstrap.png',
      "Figma": '/figma.png',
      "SASS": '/sass.png',
    },
    // Programmation
    {
      "Python": '/python.png',
      "Ruby": '/ruby.png',
      "Java": '/java.png',
      "C#": '/c_sharp.png',
      "TypeScript": '/typescript.png',
      "Go": '/go.png',
    },
    // Base de Données
    {
      "MySQL": '/mysql.png',
      "PostgreSQL": '/postgresql.png',
      "MongoDB": '/mongodb.png',
      "Firestore": '/firestore.png',
    },
    // Système/Réseau
    {
      "Windows": '/windows.png',
      "Linux": '/linux.png',
      "Serveur Linux": '/debian.png',
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
      "Docker": '/docker.png',
      "Github": '/github.png',
      "Gitlab": '/gitlab.png',
      "Microsoft Azure": 'azure.png',
    },
    // DPL/Webmarketing
    {
      "WordPress": '/wordpress.png',
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
