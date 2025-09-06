<script>
    export let imageLink = "";
    export let title = "";
    export let listTools = "";
</script>

<div class="card mb-3 h-100">
    <img src="{imageLink}" class="card-img-top mx-auto m-2" alt="certificat">
    <div class="card-body">
      <h5 class="card-title">{title}</h5>
      <p class="card-text"><small class="text-body-secondary">notions acquises : {listTools.join(', ')}</small></p>
    </div>
</div>

<style>
  img {
    max-width: 600px;
  }
</style>
  