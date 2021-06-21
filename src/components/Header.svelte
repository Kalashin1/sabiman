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
              <button class="search-submit" type="submit"
                ><i class="fa fa-chevron-right" /></button
              >
            </form>
            <button class="search-toggle" type="button"
              ><i class="fa fa-search" /></button
            >
          </div>
          <!-- HEADER SEARCH : end -->
        </div>
      </div>
      <!-- HEADER NAVIGATION : end -->
    </div>
  </div>
</header>
<!-- HEADER : end -->
