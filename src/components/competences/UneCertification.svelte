<script>
    export let imageLink = "";
    export let title = "";
    export let listTools = "";
</script>

<div class="card mb-3">
    <img src="{imageLink}" class="card-img-top" alt="...">
    <div class="card-body">
      <h5 class="card-title">{title}</h5>
      <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
      <p class="card-text"><small class="text-body-secondary">{listTools.join(', ')}</small></p>
    </div>
</div>
  