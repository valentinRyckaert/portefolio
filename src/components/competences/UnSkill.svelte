<script>
  export let skills;
</script>

<div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 row-cols-lg-4 justify-content-center">
  {#each Object.entries(skills) as [key, value]}
    <div class="col card-group g-3">
      <div class="card" style="max-width: 320px;">
        <div class="row m-2 align-items-center">
          {#if value != ''}
            <div class="col-md-4 d-flex justify-content-center">
              <img src="{value}" class="img-fluid" alt="logo {key}" style="max-height: 80px; width: auto;">
            </div>
          {/if}
          <div class="{value != '' ? "col-md-8" : "col-md-12"}">
            <div class="card-body d-flex justify-content-center align-items-center" style="height: 100%;">
              <h5 class="card-text no-break mb-0 text-center">{key}</h5>
            </div>
          </div>  
        </div>				
      </div>
    </div>
  {/each}
</div>

<style>
  img {
    max-width: 100%;
  }
</style>
  