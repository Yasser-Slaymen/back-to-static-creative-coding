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
    background-color: #072e33;
    height: 100vh;
    width: 100vw;
    overflow: hidden;
  }
  
</style>
