
<script>
    import gsap from 'gsap';
	import {ScrollTrigger} from "gsap/dist/ScrollTrigger";    
	import { onMount } from "svelte";
    onMount(() => {
        gsap.from('.sidebar-right', { duration:2, x:'-80vw', delay:'1', ease:'power2.in'})
        
    })
</script>

<div class="sidebar">
    <section class="sidebar-left">
        <ul>
            <li>itemes</li>
            <li>itemes</li>
            <li>itemes</li>
        </ul>
    </section>
    <section class="sidebar-right">
        <ul>
            <li>itemes</li>
            <li>itemes</li>
            <li>itemes</li>
        </ul>
    </section>
</div>
   
<style>
    .sidebar{
        display: flex;
        justify-content:space-between;
        width:90vw;
    }
    .sidebar-left{
        display: flex;
        justify-content:center;
        align-items: center;
        width: 10vw;
        background-color: green;
        height:50vh;
        margin-bottom: 1em;
        border-radius: .5em;

    }
    .sidebar-right{
        display: flex;
        justify-content:center;
        align-items: center;
        width: 10vw;
        height: 50vh;
        background-color: green;
        border-radius: .5em;

    }
    ul{
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        list-style-type: none;
        
    }
    li{
        background-color: rgb(6, 45, 239);
        margin: 1em;
        font-weight: 300;
        color: aliceblue;
        border-radius: .2em;
        
        padding: .5em;
    
    }

</style>

