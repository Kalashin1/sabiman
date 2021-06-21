<script>
  export let service
</script>

 <!-- SERVICE : begin -->
<li class="c-service m-type-2">
  <div class="service-inner">
    <div
      class="service-title"
      style={service.imgSrc}
    >
      <div>
        <div>
          <div>
            <span class="service-icon"
              ><i class={service.icon} /></span
            >
            <h3><a href="!#">{service.serviceTitle}</a></h3>
          </div>
        </div>
      </div>
    </div>
  </div>
</li>
<!-- SERVICE : end -->