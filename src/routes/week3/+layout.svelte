<script>
    import Border from '$lib/components/BorderAnimations.svelte'
</script>
<div class="Ap">
    <h1>Click op de Card Hieronder</h1>

    <main>
      <slot />
    </main>
    <Border/>

</div>
<style>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    .Ap{
        display: grid;
        place-items: center;
        background-color: rgb(9, 18, 81);
        width: 100vw;
        /* height: 100%; */
        height: 100vh;

    }
    h1{
        padding: .5em;
        color: aliceblue;
    }
</style>