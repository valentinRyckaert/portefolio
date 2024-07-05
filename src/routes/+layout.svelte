<script>
    import Title from "../components/layout/Title.svelte";
    import Navbar from "../components/layout/Navbar.svelte";
    import Bill from "../components/Bill.svelte";
    
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
    <div class="bg-body-secondary mt-4 text-center border-top border-dark-subtle p-5">
        <div class="row">
            <div class="col-5">
                <div class="row my-3">Valentin Ryckaert</div>
                <div class="row my-3">copyright2024</div>
                <div class="row my-3">fait avec Svelte et Bootstrap</div>
            </div>
            <div class="col-7">
                <Bill page="{activePage}"/>
                <p class="my-3">Rien sur ce site n'a été produit par IA</p>
            </div>
        </div>
    </div>
</div>



<style global>
    @import '../css/style.css';
</style>