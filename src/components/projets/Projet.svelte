<script>
    export let imageLink;
    export let imageAlt;
    export let linkTo;
    export let listTools;
</script>

<div class="card h-100" style="width: 18rem;">
    <img src="{imageLink}" class="card-img-top" alt="{imageAlt}">
    <div class="card-body">
      <h5 class="card-title">
        <slot name="title"/>
      </h5>
      <p class="card-text">
        <slot name="text"/>
      </p>
      {#if linkTo}
        <a href="{linkTo}" class="btn btn-sm btn-primary">Voir sur github</a>
      {/if}
    </div>
    <div class="card-footer">
        outils utilisés : {listTools.join(', ')}
    </div>    
</div>