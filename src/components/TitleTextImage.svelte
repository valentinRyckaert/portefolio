<script>
    export let imageLink = "";
    export let alt = "";
    export let imagePos = "";
    export let titlePos = "";
</script>

<div class="my-4">
    <div class="row">
        <h5 class="pb-2 mb-4 text-info border-bottom border-info text-{titlePos}">
            <slot name="title"/>
        </h5>
    </div>
    <div class="row">
        {#if imagePos=="left"}
            <div class="col-4">
                <img src="{imageLink}" alt="{alt}" class="img-fluid">
            </div>
            <div class="col-8">
                <slot name="body"/>
            </div>
        {:else if imagePos=="right"}
            <div class="col-8">
                <slot name="body"/>
            </div>
            <div class="col-4">
                <img src="{imageLink}" alt="{alt}" class="img-fluid">
            </div>
        {/if}
    </div>
</div>
