<script>
    import UneCertification from "./UneCertification.svelte";
</script>

<div class="row row-cols-1 row-cols-lg-2 justify-content-center g-3">
    <div class="col">
        <UneCertification imageLink="images/linux-admin.png" title="Red Hat System Administration I et II (RH124/134 - RHA) - Ver. 9.3" listTools={['Linux','RedHat Entreprise Linux (RHEL)']}/>
    </div>
    <div class="col">
        <UneCertification imageLink="images/c_FCF.png" title="Fortinet Certified Fundamentals in Cybersecurity (Fortinet)" listTools={['Cybersécurité','Pare-feux','Threat Intelligence','Sécurité applicative','Administration réseaux']}/>
    </div>
    <div class="col">
        <UneCertification imageLink="images/c_vue.png" title="Professional Vue.js Developper" listTools={['Vue.js']}/>
    </div>
    <div class="col">
        <UneCertification imageLink="images/c_python.png" title="Professional Python Developper" listTools={['Python', 'MySQL avec Python', 'MongoDB avec Python']}/>
    </div>
    <div class="col">
        <UneCertification imageLink="images/c_api_doc.png" title="Open Source Technical Documentation Essentials (Linux Fondation)" listTools={['Documentation d\'API',"Documentation Open-Source"]}/>
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
</div>