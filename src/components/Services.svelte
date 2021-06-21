<script>
  import Service from '../components/Service-Item.svelte'
  export let services = [
    {
      imgSrc: "background-image: url( 'images/cat/elec.jpg' )",
      icon: "im im-wrench",
      serviceTitle: "Plumbing",
    },
    {
      imgSrc: "background-image: url( 'images/cat/elec.jpg' )",
      icon: "im im-lightning-bolt",
      serviceTitle: "Electricity"
    },
    {
      imgSrc: "background-image: url( 'images/cat/car.jpg' )",
      icon: "im im-car",
      serviceTitle: "car hire"
    },
    {
      imgSrc: "background-image: url( 'images/cat/ed.jpg' )",
      icon: "im im-graduation-hat",
      serviceTitle: "Home Tutor"
    },
    {
      imgSrc: "background-image: url( 'images/cat/roof.jpg' )",
      icon: "im im-home",
      serviceTitle: "Roofing"
    },
    {
      imgSrc: "background-image: url( 'images/cat/food.jpg' )",
      icon: "fas fa-utensils",
      serviceTitle: "Food & Chefs"
    },
    {
      imgSrc: "background-image: url( 'images/cat/paint.jpg' )",
      icon: "im im-paintbrush",
      serviceTitle: "Painting & Decor"
    },
    {
      imgSrc: "background-image: url( 'images/cat/waste.jpg' )",
      icon: "fas fa-trash",
      serviceTitle: "wastes"
    },
    {
      imgSrc: "background-image: url( 'images/cat/shop.jpg' )",
      icon: "fas fa-shopping-cart",
      serviceTitle: "shopper"
    },
    {
      imgSrc: "background-image: url( 'images/cat/fum.jpg' )",
      icon: "fas fa-bug",
      serviceTitle: "Fumigation"
    },
    {
      imgSrc: "background-image: url( 'images/cat/sec.jpg' )",
      icon: "fas fa-shield-alt",
      serviceTitle: "Security"
    },
    {
      imgSrc: "background-image: url( 'images/cat/lun.jpg' )",
      icon: "fas fa-cloud-sun-rain",
      serviceTitle: "Laundry & Dry Cleaning"
    },
    {
      imgSrc: "background-image: url( 'images/cat/cou.jpg' )",
      icon: "im im-truck",
      serviceTitle: "COURIER"
    },
    {
      imgSrc: "background-image: url( 'images/cat/pv.jpg' )",
      icon: "fas fa-photo-video",
      serviceTitle: "Events & Media"
    },
    {
      imgSrc: "background-image: url( 'images/cat/ele.jpg' )",
      icon: "fas fa-tv",
      serviceTitle: "electronics repair"
    },
    {
      imgSrc: "background-image: url( 'images/cat/hk.jpg' )",
      icon: "fas fa-house-user",
      serviceTitle: "House Keepers"
    }
  ]
</script>

<!-- PAGE TITLE : begin -->
<div id="page-title" class="m-parallax">
  <!-- PAGE TITLE TOP : begin -->
  <div class="page-title-top">
    <div class="page-title-top-inner">
      <!-- PAGE TITLE TEXT : begin -->
      <div class="page-title-text">
        <div class="container">
          <h1>SELECT SERVICE CATEGORY</h1>
        </div>
      </div>
      <!-- PAGE TITLE TEXT : end -->

      <!-- PAGE TITLE SERVICES : begin -->
      <div class="page-title-services">
        <div class="container" style="padding-bottom:50px">
          <!-- SERVICE LIST : begin -->
          <ul class="c-service-list m-type-2 m-4-per-row">
            {#each services as service, index}
              <Service {service} />
            {/each}
          
          </ul>
          <!-- SERVICE LIST : end -->
        </div>
      </div>
      <!-- PAGE TITLE SERVICES : end -->
    </div>
  </div>
  <!-- PAGE TITLE TOP : end -->

  <!-- PAGE TITLE BOTTOM : begin -->

  <!-- PAGE TITLE BOTTOM : end -->
</div>
