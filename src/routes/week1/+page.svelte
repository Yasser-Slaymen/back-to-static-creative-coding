<script>
  import SideBar from "$lib/components/SideBar.svelte";
  import "../styles.css";
</script>

<section class="App">
  <main>
	<h1><a class="linkHeader" href="/">Back to Home page</a></h1>
    <SideBar />
  </main>
</section>

<style>
  section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100vw;
    padding: 2em;
    max-height: 70vh;
  }
  .App {
		display: flex;
		flex-direction: column;
		justify-content: center;
		min-height: 50vh;
		max-width: 100vw;
		overflow: hidden;
	}
  h1{
	position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: bold;
	width: 10em;
    height: 2em;
    margin: 0 auto;
	background-color:#050542;
	border-radius: 0.5em;
	transition: ease-out 0.3s;
	outline: none;
	z-index: 1;

  }
 .linkHeader{
	text-align: center;
    color:#66e5bf;
    font-size: 1.5rem;	
    width: inherit;
    height:inherit;
    margin-top:1.5em;
  }
  h1::before{
	content: "";
	transition:0.6s all ease;
	position: absolute;
	top: 0;
	left: 50%;
	right: 50%;
	bottom: 0;
	opacity: 0;
	background-color:#66e5bf;
	border-radius: 0.5em;
    color:#050542;

  }

  h1:hover::before{
	transition: 0.5s all ease;
	left: 0;
	right: 0;
	opacity: 1;
	z-index: -1;


  }
  .linkHeader:hover{
	color:#050542;
    text-decoration: none;
	cursor: pointer;
  } 

  

</style>
