<script>
    import Slides from "../../components/bts_sio/Slides.svelte"
    import CertifsDevProfesionnel from "./presentations/Certifs-dev-profesionnel.svelte"
    import GlpiGestionsIncident from "./presentations/GLPI-gestion-incidents.svelte"
    import WordpressDpl from "./presentations/Wordpress-DPL.svelte"
    import VeilleGraphQl from "./presentations/Veille-GraphQL.svelte"
    import PimentDispoService from "./presentations/Piment-Dispo-service.svelte"
    import ResAppliDpl from "./presentations/ResAppli-DPL.svelte"
    import PCAPRAPatrimoine from './presentations/PCA-PRA-Patrimoine.svelte'
    import ResAppliModeProjet from "./presentations/ResAppli-mode-projet.svelte"
    import OcsPatrimoine from "./presentations/OCS-Patrimoine.svelte"
    import Stage1ModeProjet from "./presentations/Stage1-mode-projet.svelte"
    import Stage2DispoService from './presentations/Stage2-Dispo-service.svelte'

    let active_presentation = 0
</script>

{#if !active_presentation}
    <h5 class="text-center mb-3">Voici le tableau de compétences présenté lors de mon BTS. Vous y trouverez les comptes rendus des TP effectués durant mes deux années d'études.</h5>
    <h6 class="text-center mb-5">(cliquez sur une case pour voir le compte rendu et accéder aux PDF.)</h6>
    <div class="table-responsive">
        <table class="table table-bordered text-center align-middle">
            <thead>
                <tr>
                    <th scope="col"></th>
                    <th scope="col">
                        Gérer le patrimoine informatique
                    </th>
                    <th scope="col">
                        Répondre aux incidents et aux demandes d'assistance et d'évolution
                    </th>
                    <th scope="col">
                        Développer la présence en ligne de l'organisation
                    </th>
                    <th scope="col">
                        Travailler en mode projet
                    </th>
                    <th scope="col">
                        Mettre à disposition des utilisateurs un service informatique
                    </th>
                    <th scope="col">
                        Organiser son développement professionnel
                    </th>
                </tr>      
            </thead>
            <tbody class="table-group-divider">
                <tr>
                    <td colspan="7" class="">
                        <p>projets en cours de formation</p>
                    </td>
                </tr>
                <tr>
                    <th scope="row">Gestion d'incidents avec GLPI</th>
                    <td></td>
                    <td on:click={() => {active_presentation = 1}} class="cross">X</td> <td></td> <td></td> <td></td> <td></td>
                </tr>
                <tr>
                    <th scope="row">Dossier de certification</th>
                    <td></td> <td></td> <td></td> <td></td> <td></td>
                    <td on:click={() => {active_presentation = 2}} class="cross">X</td>
                </tr>
                <tr>
                    <th scope="row">Développement de présence en ligne</th>
                    <td></td> <td></td>
                    <td on:click={() => {active_presentation = 3}} class="cross">X</td>
                    <td></td> <td></td> <td></td>
                </tr>
                <tr>
                    <th scope="row">Développement de l'application ResAppli</th>
                    <td></td> <td></td>
                    <td on:click={() => {active_presentation = 4}} class="cross">X</td>
                    <td on:click={() => {active_presentation = 5}} class="cross">X</td>
                    <td></td> <td></td>
                </tr>
                <tr>
                    <th scope="row">Application web Piment</th>
                    <td></td> <td></td> <td></td> <td></td>
                    <td on:click={() => {active_presentation = 6}} class="cross">X</td>
                    <td></td>
                </tr>
                <tr>
                    <th scope="row">Gestion d'inventaire OCS Inventory</th>
                    <td on:click={() => {active_presentation = 7}} class="cross">X</td>
                    <td></td> <td></td> <td></td> <td></td> <td></td>
                </tr>
                <tr>
                    <th scope="row">Veille technologique sur le GraphQL</th>
                    <td></td>
                    <td></td> <td></td> <td></td>
                    <td></td>
                    <td on:click={() => {active_presentation = 8}} class="cross">X</td>
                </tr>
                <tr>
                    <th scope="row">TP PCA-PRA (gouvernance)</th>
                    <td on:click={() => {active_presentation = 9}} class="cross">X</td>
                    <td></td> <td></td> <td></td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td colspan="7" class="">
                        <p>projets durant le stage de première année</p>
                    </td>
                </tr>
                <tr>
                    <th scope="row">Développement de fonctionnalités web</th>
                    <td></td> <td></td>
                    <td></td>
                    <td on:click={() => {active_presentation = 10}} class="cross">X</td>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td colspan="7" class="">
                        <p>projets durant le stage de seconde année</p>
                    </td>
                </tr>
                <tr>
                    <th scope="row">Application web NPSA-NG</th>
                    <td></td> <td></td> <td></td> <td></td>
                    <td on:click={() => {active_presentation = 11}} class="cross">X</td>
                    <td></td>
                </tr>
            </tbody>    
        </table>
    </div>
{:else}
    {#if active_presentation === 1}
        <Slides nbPages=12 bind:active_presentation documents={['compte-rendu-GLPI.pdf', 'Documentation-installation-GLPI.pdf']}>
            <GlpiGestionsIncident/>
        </Slides>
    {:else if active_presentation === 2}
        <Slides nbPages=7 bind:active_presentation documents={['Projet-Professionnel-SIO1.pdf', 'Projet-Professionnel-SIO2.pdf']}>
            <CertifsDevProfesionnel/>
        </Slides>
    {:else if active_presentation === 3}
        <Slides nbPages=7 bind:active_presentation documents={['Dossier_VotreGouvernement.pdf']}>
            <WordpressDpl/>
        </Slides>
    {:else if active_presentation === 4}
        <Slides nbPages=7 bind:active_presentation documents={['documentation-utilisateur-ResAppli.pdf', 'presentation-commerciale-ResAppli.pdf']}>
            <ResAppliDpl/>
        </Slides>
    {:else if active_presentation === 5}
        <Slides nbPages=6 bind:active_presentation documents={['documentation-utilisateur-ResAppli.pdf', 'presentation-commerciale-ResAppli.pdf']}>
            <ResAppliModeProjet/>
        </Slides>
    {:else if active_presentation === 6}
        <Slides nbPages=7 bind:active_presentation>
            <PimentDispoService/>
        </Slides>
    {:else if active_presentation === 7}
        <Slides nbPages=8 bind:active_presentation documents={['Compte-Rendu-OCS-Inventory.pdf']}>
            <OcsPatrimoine/>    
        </Slides>
    {:else if active_presentation === 8}
        <Slides nbPages=8 bind:active_presentation documents={['Les-API-GraphQL.pdf']}>
            <VeilleGraphQl/>
        </Slides>
    {:else if active_presentation === 9}
        <Slides nbPages=8 bind:active_presentation documents={['Compte-Rendu-PRA.pdf', 'PRA-PRASN.pdf']}>
            <PCAPRAPatrimoine/>
        </Slides>
    {:else if active_presentation === 10}
        <Slides nbPages=6 bind:active_presentation documents={['rapport-de-stage-SIO-1.pdf']}>
            <Stage1ModeProjet/>
        </Slides>
    {:else if active_presentation === 11}
        <Slides nbPages=6 bind:active_presentation documents={['rapport-de-stage-SIO2.pdf']}>
            <Stage2DispoService/>  
        </Slides>
    {/if}
{/if}

<style>
    .cross:hover {
        background-color: lightgray
    }
</style>