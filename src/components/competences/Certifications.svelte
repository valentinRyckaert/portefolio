<script>
    import UneCertification from "./UneCertification.svelte";
</script>

<div class="row row-cols-1 row-cols-lg-2 justify-content-center g-3">
    <div class="col">
        <UneCertification imageLink="images/c_api_doc.pdf" title="Open Source Technical Documentation Essentials (Linux Fondation)" listTools={['Documentation d\'API',"Documentation Open-Source"]}/>
    </div>
    <div class="col">
        <UneCertification imageLink="images/c_backend.png" title="Backend development and APIs (FreeCodeCamp)" listTools={["Node.js","Express.js","MongoDB"]}/>
    </div>
    <div class="col">
        <UneCertification imageLink="images/c_anssi.png" title="MOOC cybersécurité (ANSSI)" listTools={["sécurité des mots de passe","sécurité physique","preuve informatique","bonnes pratiques cyber"]}/>
    </div>
    <div class="col">
        <UneCertification imageLink="images/c_vigipirate.jpg" title="Faire Face Ensemble (SGDSN)" listTools={["sécurité citoyenne"]}/>
    </div>
    <div class="col">
        <UneCertification imageLink="images/c_cloud.jpg" title="Description des concpets du Cloud (Microsoft Learn)" listTools={["cloud computing"]}/>
    </div>
    <div class="col">
        <UneCertification imageLink="images/c_ubuntu.jpg" title="Linux Ubuntu : Les Fondamentaux (Skilleos)" listTools={["Linux","Ubuntu Server"]}/>
    </div>
    <div class="col">
        <UneCertification imageLink="images/c_svelte.jpg" title="Svelte.js 3 (Skilleos)" listTools={["Svelte"]}/>
    </div>
</div>