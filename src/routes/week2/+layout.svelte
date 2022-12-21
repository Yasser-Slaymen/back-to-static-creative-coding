<script>
  import Footer2 from "$lib/components/Footer2.svelte";
</script>

<div class="App">
  <main>
    <Footer2/>
    <!-- <Head2 /> -->
    <slot />
  </main>
</div>

<style>
  .App {
    display: flex;
    justify-content: space-around;
    align-items: center;
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
