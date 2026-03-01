<script>
  import UnSkill from "./UnSkill.svelte";

  let skillFamilyList = [
    "Web",
    "Programmation",
    "Base de données",
    "Système/Réseau",
    "Virtualisation",
    "Cybersécurité",
    "DevOps",
    "DPL/Webmarketing",
    "Soft Skills",
    "Langues",
    "Linux",
    "Outils"
  ];

  let skillsDictionnary = [
    // Web
    {
      "React": 'images/React.png',
      "Svelte": 'images/svelte.svg',
      "FastAPI": 'images/fastapi.png',
      "Deno": 'images/deno.png',
      "Vue.js": 'images/vue.png',
      "Node.js": 'images/nodejs.png',
      "Express": 'images/nodejs.png',
      "Angular": 'images/angular.png',
      "Django": 'images/django.png',
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
      "C": 'images/C.png',
      "PHP": 'images/php.png',
      "TypeScript": 'images/typescript.png',
      "Go": 'images/go.png',
    },
    // Base de Données
    {
      "MariaDB": 'images/mariadb.png',
      "PostgreSQL": 'images/postgresql.png',
      "OracleDB": 'images/oracledb.png',
      "MongoDB": 'images/mongodb.png',
      "Firestore": 'images/firestore.png',
    },
    // Système/Réseau
    {
      "Windows": 'images/windows.png',
      "Linux": 'images/linux.png',
      "Serveur Linux": 'images/debian.png',
      "DNS": '',
      "DHCP": '',
      "Routage": '',
      "VLAN": '',
      "Cisco": '',
      "Switching": '',
      "VLSM/FLSM": ''
    },
    // Virtualisation
    {
      "VMWare": 'images/vmware.jpg',
      "vSphere": 'images/vmware-vsphere.svg',
      "Qemu/KVM": 'images/QEMU.png',
    },
    // Cybersécurité
    {
      "OPNSense": 'images/opnsense.svg',
      "WAF": 'images/logo-safeline.png',
      "Horodatage": '',
      "Chiffrement": '',
      "Sécurité Réseaux": '',
      "Sécurité applicative": '',
      "Bonnes pratiques cyber": ''
    },
    // DevOps
    {
      "Docker": 'images/docker.png',
      "Github": 'images/github.png',
      "Gitlab": 'images/gitlab.png',
      "Apache": 'images/apache.svg'
    },
    // DPL/Webmarketing
    {
      "WordPress": 'images/wordpress.png',
      "Référencement/SEO": '',
      "E-mailing": '',
    },
    // Soft Skills
    {
      "Autoapprenissage": '',
      "Travail en équipe": '',
      "Conduite de projet": '',
      "Bon relationnel": ''
    },
    // Langues
    {
      "Anglais": '',
      "Allemand": '',
    },
    // Linux
    {
      "Arch": 'images/arch.svg',
      "Fedora": 'images/fedora.svg',
      "Ubuntu": 'images/ubuntu.svg',
      "Debian": 'images/debian.svg',
      "RHEL": 'images/redhat.svg',
      "Kali": 'images/kali.svg',
      "Alpine": 'images/alpine-linux.png'
    },
    
    // Outils
    {
      "Obsidian": 'images/obsidian.png',
      "Only office": 'images/onlyoffice.png',
      "Suite office": 'images/suite-office.png',
      "VsCode": 'images/vscode.png',
      "IntelliJ": 'images/intellij.png',
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
        {:else if active == skillFamilyList[11]}
          <UnSkill skills={skillsDictionnary[11]}/>
        {/if}
    </div>
</div>
