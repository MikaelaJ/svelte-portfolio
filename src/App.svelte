<script>
  import WorkList from "./components/WorkList.svelte";
	import Header from "./components/Header.svelte";
	import Footer from "./components/Footer.svelte";
	import FrameWorks from "./components/FrameWorks.svelte";

</script>

<svelte:head>
  <link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap" rel="stylesheet">
<link href="http://fonts.cdnfonts.com/css/neon-80s" rel="stylesheet">
                
                
</svelte:head>

<header>
	<Header />
</header>
<main>
	<WorkList />
	<FrameWorks />
</main>
<footer>
	<Footer />
</footer>

<style>
  :global(:root) {
		--bg: #202426;
		--grey: #8c8c88;
		--light: #f2f2f2;
		--neonPink: #f24987ab;
    font-family: 'Roboto', sans-serif;
	}

	:global(body) {
		background: var(--bg);
		background-image: url("/assets/img/noise-light.png");
		color: var(--light);
    width: inherit; 
    min-height: inherit; 
    margin: 0; 
    padding: 0; 
	}

  :global(a) {
    text-decoration: none;
  }
  :global(html) { 
      width: 100%; 
      min-height: 100%; 
  } 
  :global(*) { 
    box-sizing: border-box; 
} 
 
 
/* body { 
    width: inherit; 
    min-height: inherit; 
    margin: 0; 
    padding: 0; 
} */
  
  main {
    max-width: 1024px;
    margin: 0 auto;
  }

	header {
        margin: 0% 0% 5% 0%;
	}
  @media (max-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
