<script>
    export let imagePos="right";
    export let imageLink="";
    export let alt="";
</script>

{#if imagePos === "right"}
    <div class="col-lg p-4 border border-5 rounded-5 my-auto text-center">
        <slot/>
    </div>
    <div class="col-lg">
        <img src="{imageLink}" class="img-fluid" alt="{alt}">
    </div>
{:else}
    <div class="col-lg">
        <img src="{imageLink}" class="img-fluid" alt="{alt}">
    </div>
    <div class="col-lg p-4 border border-5 rounded-5 my-auto text-center">
        <slot/>
    </div>
{/if}

<style>
    img {
      max-width: 400px;
      display: block;
      margin-left: auto;
      margin-right: auto;
    }
</style>
    