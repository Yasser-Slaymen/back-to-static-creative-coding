<script>
  import Head2 from "$lib/components/Head2.svelte";
  import Footer2 from "$lib/components/Footer2.svelte";
</script>

<div class="App">
  <main>
    <Head2 />
    <slot />
    <Footer2/>
  </main>
</div>

<style>
  .App {
    background-image: url($lib/images/pex.jpg);
    background-size:cover;
    object-fit: cover;
    background-position: center;
    background-repeat: no-repeat;
    height: 100vh;
    width: 100vw;
    overflow: hidden;
  }
  
</style>
