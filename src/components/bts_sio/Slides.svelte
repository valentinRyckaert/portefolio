<script>
  export let nbPages
</script>

<div class="card">
    <div class="card-body">
        <div id="carouselIndicators" class="carousel carousel-dark slide">
            <div class="carousel-indicators">
              <button type="button" data-bs-target="#carouselIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
              {#each {length: nbPages-1} as _, i}
                <button type="button" data-bs-target="#carouselIndicators" data-bs-slide-to={i+1} aria-label="Slide {i+1}"></button>
              {/each}
            </div>
            <div class="carousel-inner pb-5" style="padding-inline: 130px;">
                <slot/>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselIndicators" data-bs-slide="prev">
              <span class="carousel-control-prev-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselIndicators" data-bs-slide="next">
              <span class="carousel-control-next-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Next</span>
            </button>
        </div>
    </div>
</div>
