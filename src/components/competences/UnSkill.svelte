<script>
    export let skills;
</script>

<div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 row-cols-lg-4 justify-content-center">
    {#each Object.entries(skills) as skill}
        <div class="col card-group g-3">
            <div class="card mb-3" style="max-width: 320px;">
                <div class="row">
                  {#if skill[1][0] != ''}
                    <div class="col-md-4">
                      <img src="{skill[1][0]}" class="img-fluid m-2 " alt="logo {skill[0]}">
                    </div>
                  {/if}
                  <div class="{skill[1][0] != '' ? "col-md-8" : ""}">
                    <div class="card-body">
                      <h5 class="card-text no-break">{skill[0]}</h5>
                    </div>
                  </div>
                </div>
                <div class="card-footer mt-auto text-body-secondary">
                  expérience : {skill[1][1]}
                </div>					
            </div>
        </div>
    {/each}
</div>