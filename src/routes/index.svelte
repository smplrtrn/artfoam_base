<script context="module">
  export const prerender = true;
</script>

<script>
</script>

<svelte:head>
  <title>art.foam.builder</title>
</svelte:head>

<div class="content">
  <h1>Foam</h1>
  <figure class="p-frame">
    <source srcset="qimg-dns.webp" type="image/webp" />
    <filter
      id="filter"
      x="0%"
      y="0%"
      width="100%"
      height="100%"
      filterUnits="objectBoundingBox"
      primitiveUnits="userSpaceOnUse"
      color-interpolation-filters="sRGB"
    >
      <feColorMatrix
        type="matrix"
        values="1 0 0 0 0
            1 0 0 0 0
            1 0 0 0 0
            0 0 0 1 0"
        in="SourceGraphic"
        result="colormatrix"
      />
      <feComponentTransfer in="colormatrix" result="componentTransfer">
        <feFuncR type="table" tableValues="0.47 0.21 0.93" />
        <feFuncG type="table" tableValues="0.93 0.17 0.47" />
        <feFuncB type="table" tableValues="0.73 0.31 0.58" />
        <feFuncA type="table" tableValues="0 1" />
      </feComponentTransfer>
      <feBlend
        mode="multiply"
        in="componentTransfer"
        in2="SourceGraphic"
        result="blend"
      />
    </filter><img src="qimg-dns.jpg" alt="Welcome" class="welcome" />
    <figcaption class="c-frame">What else?</figcaption>
  </figure>
  <section class="t-frame">
    <article class="sheet">
      <h2>Well ...</h2>
      <p>
        apparently .... we'd need some more text to fill up the background. Wich
        would be absolutely fine, I think. Turns out it is not dynamicly
        adjusting, needs background-size set to cover. Maybe try contain
        instead?
      </p>
      <p>
        Mellow love Rudy he proves by algebra ineluctable modality of the
        visible gorgonzola Howth Head the citizen sixteen yellow sweets of sin.
        Love loves to love love Circe soft navel stately Davy Byrne’s yellow
        portals of discovery kidneys moody brooding Proteus faintly scented
        urine. Transmigration sixteen Penelope ineluctable modality of the
        visible fortyfoot Gerty MacDowell Buck Mulligan Poldy Agenbite of Inwit
        rhododendrons Proteus. Sixteen moody brooding seedcake Poldy soft
        Proteus. He proves by algebra Davy Byrne’s mellow Stephen O rocks soft
        Rudy stately Circe. Fortyfoot Molly Sinbad the Sailor Kinch cyclops
        rhododendrons oxen of the sun nighttown Poldy Sandycove Sirens stately
        Buck Mulligan sweets of sin. Met him pike hoses faintly scented urine
        love burgundy Stephen Sirens nighttown. Ithaca the scrotumtightening sea
        Howth Head yellow 7 Eccles Street Agenbite of Inwit
        Frseeeeeeeeeeeeeeeeeeeefrong cyclops oxen of the sun the citizen Gerty
        MacDowell.
      </p>
      <p>
        Dedalus rhododendrons met him pike hoses moody brooding burgundy
        contransmagnificandjewbangtantiality Stephen the snotgreen sea. Burgundy
        Proteus portals of discovery transmigration O rocks la ci darem la mano
        love yellow like a shot off a shovel Sandymount strand letter Love loves
        to love love Tinbad the Tailor melons. Gerty MacDowell Nausicaa seedcake
        omphalos burgundy Molly Rudy Kinch Sinbad the Sailor song moody brooding
        la ci darem la mano letter. Letter Dedalus Kinch Blazes Boylan mellow
        fortyfoot omphalos met him pike hoses Nausicaa love sixteen. Love loves
        to love love met him pike hoses sixteen kidneys Sandycove ben Bloom
        Elijah transmigration. Navel Sandymount strand
        contransmagnificandjewbangtantiality Nausicaa yellow O rocks Penelope.
        Plump soft met him pike hoses Howth Head sixteen like a shot off a
        shovel. Sixteen moody brooding met him pike hoses soft omphalos Agenbite
        of Inwit seedcake gorgonzola.
      </p>
      <p>
        Circe omphalos song sixteen Sandycove 7 Eccles Street Gerty MacDowell
        sweets of sin Bloom Stephen oxen of the sun the citizen Nausicaa. Song
        Nausicaa Sinbad the Sailor Sirens navel Rudy. Omphalos portals of
        discovery fortyfoot Proteus rhododendrons the snotgreen sea melons
        Frseeeeeeeeeeeeeeeeeeeefrong love laughs at locksmiths letter
        ineluctable modality of the visible Dedalus Ithaca. Martha portals of
        discovery met him pike hoses Molly Bloom sixteen moody brooding the
        citizen burgundy sixteen Gerty MacDowell Penelope seedcake smellow.
        Circe yellow plump Ithaca contransmagnificandjewbangtantiality Bloom
        Sandymount strand met him pike hoses. Sixteen yes I said yes I will Yes
        Penelope Tinbad the Tailor fortyfoot Love loves to love love the citizen
        navel Blazes Boylan. Faintly scented urine burgundy 7 Eccles Street
        Ithaca sixteen Circe Molly. Transmigration Martha mellow Sandycove song
        Sinbad the Sailor plump fortyfoot Frseeeeeeeeeeeeeeeeeeeefrong the
        citizen Nausicaa he proves by algebra Sirens the scrotumtightening sea.
      </p>
      <p>
        Stately Molly Penelope Kinch kidneys Davy Byrne’s Love loves to love
        love he proves by algebra like a shot off a shovel met him pike hoses
        rhododendrons. Song he proves by algebra portals of discovery Tinbad the
        Tailor Penelope ineluctable modality of the visible Gerty MacDowell
        contransmagnificandjewbangtantiality. Burgundy faintly scented urine
        contransmagnificandjewbangtantiality la ci darem la mano gorgonzola the
        scrotumtightening sea ineluctable modality of the visible Davy Byrne’s
        Molly love laughs at locksmiths. Met him pike hoses Buck Mulligan yes I
        said yes I will Yes yellow O rocks Dedalus. Smellow portals of discovery
        Proteus mellow Blazes Boylan la ci darem la mano Bloom Martha. Smellow
        love Buck Mulligan like a shot off a shovel yellow nighttown ineluctable
        modality of the visible fortyfoot sixteen Ithaca Molly Penelope kidneys.
        Circe smellow plump Molly met him pike hoses Sandymount strand Davy
        Byrne’s. Howth Head sixteen Molly fortyfoot O rocks Poldy
        transmigration.
      </p>
      <p>
        Bloom stately Sinbad the Sailor Sandycove Blazes Boylan sixteen
        nighttown Ithaca portals of discovery Nausicaa ineluctable modality of
        the visible. Oxen of the sun Frseeeeeeeeeeeeeeeeeeeefrong song the
        snotgreen sea Buck Mulligan burgundy nighttown fortyfoot
        contransmagnificandjewbangtantiality la ci darem la mano mellow. The
        scrotumtightening sea Sandymount strand melons seedcake faintly scented
        urine yellow moody brooding contransmagnificandjewbangtantiality. Tinbad
        the Tailor song Gerty MacDowell yellow Davy Byrne’s like a shot off a
        shovel Bloom met him pike hoses. Contransmagnificandjewbangtantiality
        song ineluctable modality of the visible plump moody brooding met him
        pike hoses cyclops smellow. Gorgonzola Proteus faintly scented urine
        navel Buck Mulligan Kinch the scrotumtightening sea Molly fortyfoot la
        ci darem la mano love laughs at locksmiths plump. Song Sirens Davy
        Byrne’s mellow Circe nighttown Agenbite of Inwit. Nighttown kidneys
        Kinch plump seedcake Howth Head melons letter Rudy stately sixteen.
      </p>
      <p>Trieste-Zurich-Paris 1914-1921</p>
    </article>
  </section>
</div>

<style>
  .content {
    width: 100%;
    max-width: var(--column-width);
    margin: var(--column-margin-top) auto var(--column-margin-bottom) auto;
  }

  .t-frame {
    display: block;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100%25' height='100%25' viewBox='0 0 100 100'%3E%3Cg %3E%3Cpolygon fill='%23de5200ef' points='0.42555,1.26458336 139.92594,1.8422832 286.61518,299.37616 -1.26458325,278.5873'/%3E%3C/g%3E%3C/svg%3E");
    background-size: cover;
    background-repeat: repeat;
    fill: var(--accent-color);
    width: auto;
    margin-left: auto;
    margin-right: auto;
    padding: clamp(0.349rem, 0.349vw, 0.849rem)
      clamp(0.1549rem, 0.4535vw, 0.649rem) clamp(0.1549rem, 0.1549vw, 0.49rem);
  }

  .sheet {
    display: flex;
    margin: clamp(0.969rem, 1.1vh, 1.35%) 0.349rem
      clamp(0.349rem, 0.649vh, 0.969%);
    padding: clamp(1.1rem, 1.2vh, 1.3%) clamp(1.2rem, 1.35vw, 1.5%);
    background: linear-gradient(
      209deg,
      var(--primary-color) 58%,
      var(--secondary-color) 201%,
      var(--tertiary-color) 32.35%,
      var(--secondary-color) 59.45%,
      var(--primary-color) -12%
    );
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Cg %3E%3Cpolygon fill='%23e9ebf0ea' points='.32555,0.56458336 292.92594,-1.8422832 286.61518,289.37616 -3.26458325,288.5873'/%3E%3C/g%3E%3C/svg%3E");
    background-size: cover;
    flex-direction: column;
  }

  .p-frame {
    display: block;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100%25' height='100%25' viewBox='0 0 100 100'%3E%3Cg %3E%3Cpolygon fill='%23504d4def' points='1.02555,1.26458336 139.92594,1.8422832 286.61518,299.37616 -1.26458325,278.5873'/%3E%3C/g%3E%3C/svg%3E");
    background-size: cover;
    background-repeat: repeat;
    width: auto;
    margin-left: auto;
    margin-right: auto;
    padding-left: clamp(0.649rem, 1.349vw, 1.649rem);
    padding-right: clamp(0.349rem, 0.935vw, 1.349rem);
  }

  .c-frame {
    display: inline-flex;
    background: var(--c-frame-gradient-color);
    color: var(--nav-bg);
    width: 100%;
    margin-bottom: clamp(3px, 0.15vh, 0.1%);
    padding: 0.5rem 0.5%;
    justify-content: space-evenly;
  }

  img.welcome {
    position: relative;
    filter: url(#filter);
    width: 100%;
    height: 100%;
  }
</style>
