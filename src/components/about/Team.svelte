<script>
  export let teamMates = [
    {
      name: "John Handy",
      role: "Plumbing, Sanitary, Sewerage",
      description:
        "The copy warned the Little Blind Text, that where it came from it would have been rewritten a thousand times and everything that was left from.",
      picture: "images/team-member-01.jpg",
      social: {
        twitter: "twitter-link",
        linkedIn: "linkedIN",
      },
    },
    {
      name: "Keith Skilful",
      role: "Heating, Electricity",
      description:
        " Bookmarksgrove, the headline of Alphabet Village and the subline of  her own road, the Line Lane. Pityful a rethoric question ran over  her cheek.",
      picture: "images/team-member-02.jpg",
      social: {
        twitter: "twitter",
        linkedIn: "linkedin",
      },
    },
    {
      name: "Mick Nifty",
      role: "Roofing, Renovation",
      description:
        " But nothing the copy said could convince her and so it didn’t take  long until a few insidious Copy Writers ambushed her, made her drunk with.",
      picture: "images/team-member-04.jpg",
      social: {
        twitter: "twitter",
        linkedIn: "linkedin",
      },
    },
    {
      name: "Joe Slick",
      role: "Painting, Electricity",
      description:
        "A small river named Duden flows by their place and supplies it with  the necessary regelialia. It is a paradisematic country, in which  roasted parts.",
      picture: "images/team-member-04.jpg",
      social: {
        twitter: "twitter",
        linkedIn: "linkedin",
      },
    },
  ];
</script>

<section>
  <h2>Our <strong>Team</strong></h2>

  <div class="row">
    {#each teamMates as teamMate, index}
      <div class="col-md-6">
        <!-- TEAM MEMBER : begin -->
        <div class="c-team-member m-has-portrait">
          <div class="member-portrait">
            <img src={teamMate.picture} alt="" />
          </div>
          <h3 class="member-name">{ teamMate.name }</h3>
          <h4 class="member-role">{ teamMate.role }</h4>
          <div class="member-description">
            <p>
              { teamMate.description }
            </p>
          </div>
          <ul class="member-social">
            <li>
              <a href={teamMate.social.twitter} title="Twitter"><i class="fa fa-twitter" /></a>
            </li>
            <li>
              <a href={teamMate.social.linkedIn} title="LinkedIn"><i class="fa fa-linkedin" /></a>
            </li>
          </ul>
        </div>
        <!-- TEAM MEMBER : end -->
        <hr class="c-divider m-transparent hidden-md hidden-lg" />
      </div>
    {/each}
  </div>
</section>
