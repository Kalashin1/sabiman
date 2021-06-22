<script>
  import ContactForm from './Contact-form.svelte'
</script>

<div class="container">
  <!-- PAGE CONTENT : begin -->
  <div id="page-content">
    <div class="row">
      <div class="col-md-4">
        <!-- ICON BLOCK : begin -->
        <div class="c-icon-block">
          <i class="im im-compass" />
          <h3>Our HQ</h3>
          <p>
            Mgbuakara, Elioparanwo,<br />
            Port Harcourt, Rivers State, Nigeria.<br />
          </p>
        </div>
        <!-- ICON BLOCK : end -->

        <hr class="c-divider" />

        <!-- ICON BLOCK : begin -->
        <div class="c-icon-block">
          <i class="im im-clock2" />
          <h3>Opening Hours</h3>
          <p>
            <strong>Mon. - Fri.:</strong> 7am - 5pm<br />
            <strong>Saturday:</strong> 10am - 4pm<br />
            <strong>Sunday:</strong> Closed
          </p>
        </div>
        <!-- ICON BLOCK : end -->

        <hr class="c-divider" />

        <!-- ICON BLOCK : begin -->
        <div class="c-icon-block">
          <i class="im im-phone" />
          <h3>24/7 Support</h3>
          <p>
            08066926113<br />
            <a href="!#">hello@sabiman.ng</a>
          </p>
        </div>
        <!-- ICON BLOCK : end -->

        <hr class="c-divider m-transparent hidden-lg hidden-md" />
      </div>
      <div class="col-md-8">
        <!-- GOOGLE MAP : begin -->
        <!-- If you specify the "data-address" attribute, "data-latitude" and "data-longitude" are optional -->
        <!-- API KEY IS REQUIRED! More info https://developers.google.com/maps/documentation/javascript/get-api-key -->
        <div
          class="c-gmap"
          data-google-api-key="YOUR-API-KEY"
          data-address="8833 Sunset Blvd, West Hollywood, CA 90069, USA"
          data-latitude="34.0909191"
          data-longitude="-118.38417279999999"
          data-zoom="18"
          data-maptype="satellite"
          data-enable-mousewheel="false"
        />
        <!-- GOOGLE MAP : end -->
      </div>
    </div>

    <hr class="c-divider m-size-medium" />

    <h2 style="text-align: left">Get More Info, <strong>Request a Quote</strong> or Just Say Hi</h2>
    <ContactForm />
  </div>
  <!-- PAGE CONTENT : end -->
</div>
