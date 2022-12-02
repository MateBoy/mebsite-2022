<svelte:head>
	<title>MateBoy | Home</title>
  <meta name="description" content="The start page of Swedish front end developer MateBoy">
</svelte:head>

<div class="intro">
    <div class="intro__text">
        <h1 class="kanji">神贈</h1>
        <h1 class="headline">Hello, I'm MateBoy. I'm a <em>front end developer</em> based in Stockholm, <span class="swe">Sweden</span>.</h1>

        <p>
        I have five years of experience working with HTML, CSS and JavaScript. When I'm not writing code, I enjoy <a href="https://last.fm/user/MeTRoD">listening to music</a>, <a href="https://www.discogs.com/user/MateBoy/collection">collecting vinyl records</a>, <a href="https://www.backloggd.com/u/MateBoy/">playing video games</a>, <a href="https://letterboxd.com/MateBoy/">and watching movies</a>.
        </p>
        <p>
        Currently I work as a consultant at <a href="https://www.majority.com">MAJORITY</a>, via <a href="https://nexergroup.com">Nexer</a>.
        </p>
    </div>
    <picture>
      <source srcset="./assets/memojidec22.webp" type="image/webp">
      <img src="./assets/memojidec22.png" class="intro__image" alt="Me as a Memoji" width="250" height="250">
    </picture>
</div>

<style>
  .kanji {
    font-size: 4rem;
    margin-top: 0;
    padding: 1.5rem;
    background: rgba(0, 0, 0, 0.2);
    display: inline-block;
    line-height: normal;
  }

  .intro__image {
    width: 275px;
    margin-left: auto;
    margin-right: auto;
    display: block;
  }

  @media screen and (min-width: 768px) {
    .intro {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
    }

    .intro__text {
      max-width: 52rem;
      flex-shrink: 1;
    }

    .intro__image {
      width: 25rem;
      flex-grow: 1;
    }
  }
</style>