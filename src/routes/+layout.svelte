<script>
    import Title from "../components/layout/Title.svelte";
    import Navbar from "../components/layout/Navbar.svelte";
    
    let activePage = '/';
</script>

<div>
    <div class="container">
        <div class="row mt-5">
            <Title/>
        </div>
        <div class="row mt-2 mb-5">
            <Navbar bind:active="{activePage}"/>
        </div>
        <slot/>
    </div>
    <br>
    <div class="bg-body-secondary text-center mt-3 border-top border-dark-subtle p-4">
        <p class="my-1">Contact : <a href="mailto:valentin.ryckaert@protonmail.com">valentin.ryckaert@protonmail.com</a></p>
        <p class="my-3">Copyright © 2024 Valentin Ryckaert - tous droits réservés</p>
        <p class="my-1">Fait avec Svelte et Bootstrap</p>
    </div>
</div>