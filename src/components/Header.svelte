<script>
  export let segment
  const links = [ 
    {
      link: "",
      text: 'home'
    },
    {
      link: "about",
      text: 'about sabiman'
    },
    {
      link: "contact",
      text: 'contact'
    },
  ]

  const handleClick = () => {
    console.log(segment)
  }
</script>

<style>
  /* .active {
    color: dimgrey;
    border-color: #ffb617;
  } */
</style>

<!-- HEADER : begin -->
<header id="header">
  <div class="header-inner">
    <div class="container">
      <!-- HEADER BRANDING : begin -->
      <div class="header-branding">
        <div class="branding-inner">
          <!-- BRANDING LOGO : begin -->
          <div class="brading-logo">
            <a href="/" on:click={handleClick}
              ><img
                src="images/logo.png"
                data-hires="images/logo.2x.png"
                alt="Blue Collar"
              /></a
            >
          </div>
          <!-- BRANDING LOGO : end -->

          <!-- BRANDING INFO : begin -->
          <div class="brading-info" on:click={handleClick}>
            <strong style="color:purple">SabiMan</strong><br />
            <em>Premium Service Market</em>
          </div>
          <!-- BRANDING INFO : end -->
        </div>
      </div>
      <!-- HEADER BRANDING : end -->

      <!-- NAVIGATION TOGGLE : begin -->
      <button class="header-navigation-toggle" type="button"
        ><i class="fa fa-bars" /></button
      >
      <!-- NAVIGATION TOGGLE : end -->

      <!-- HEADER NAVIGATION : begin -->
      <div class="header-navigation">
        <div class="navigation-inner">
          <!-- HEADER MENU : begin -->
          <nav class="header-menu">
            <ul>
              
              {#each links as link }
                <li>
                  <a href={link.link} class:m-active={segment==link.link}>{ link.text }</a>
                </li>
              {/each}
            </ul>
          </nav>
          <!-- HEADER MENU : end -->

          <!-- HEADER SEARCH : begin -->
          <div class="header-search">
            <form action="search-results.html">
              <input
                class="search-input"
                type="text"
                placeholder="Search for..."
              />
              <button class="search-submit" type="submit">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="#ffc107" viewBox="0 0 24 24"><path d="M10 6L8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"/></svg>
              </button>
            </form>
            <button class="search-toggle" type="button">
              <svg xmlns="http://www.w3.org/2000/svg" fill="#ffc107" width="24" height="24" viewBox="0 0 24 24"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"/></svg>
            </button>
          </div>
          <!-- HEADER SEARCH : end -->
        </div>
      </div>
      <!-- HEADER NAVIGATION : end -->
    </div>
  </div>
</header>
<!-- HEADER : end -->
