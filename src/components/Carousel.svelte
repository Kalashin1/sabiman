<script>
  const items = [
    "images/sli/coro.png",
    "images/sli/lun.png",
    "images/sli/rel.png",
    "images/sli/twn.png",
    "images/sli/hw.png",
    "images/sli/time.png",
  ];
</script>

<div
  class="container shadow p-0 mb-5 bg-white rounded-lg"
  style="margin-top:20px"
>
  <div id="carouselExampleControls" class="carousel slide" data-ride="carousel">
    <div class="carousel-inner">
      {#each items as item, index}
        {#if index === 0}
          <div class="carousel-item active">
            <img src={item} class="d-block w-100 rounded" alt="..." />
          </div>
        {/if}
        <div class="carousel-item">
          <img src={item} class="d-block w-100 rounded" alt="..." />
        </div>
      {/each}
    </div>
  </div>
</div>
