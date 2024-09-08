<script>
    export let imageLink = "";
    export let alt = "";
    export let imagePos = "";
    export let titlePos = "";
</script>

<div class="my-4">
    <div class="row">
        <h5 class="pb-2 mb-4 text-primary-emphasis border-bottom border-primary text-{titlePos}">
            <slot name="title"/>
        </h5>
    </div>
    <div class="row">
        {#if imagePos=="left"}
            <div class="col-lg-4">
                <img src="{imageLink}" alt="{alt}" class="img-fluid my-3">
            </div>
            <div class="col-lg-8">
                <slot name="body"/>
            </div>
        {:else if imagePos=="right"}
            <div class="col-lg-8">
                <slot name="body"/>
            </div>
            <div class="col-lg-4">
                <img src="{imageLink}" alt="{alt}" class="img-fluid my-3">
            </div>
        {/if}
    </div>
</div>

<style>
    img {
      max-width: 300px;
      display: block;
      margin-left: auto;
      margin-right: auto;
    }
</style>
    