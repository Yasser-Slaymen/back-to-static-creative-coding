<script>
    import {gsap} from 'gsap';
	import {ScrollTrigger} from "gsap/dist/ScrollTrigger";    
	import { onMount } from "svelte";
    onMount(() => {
        gsap.from('nav', { duration:1.5, y: '-100%', ease:'bounce'})
         gsap.from('.listItems-nav', { duration:1.5, opacity: 0, delay: 1,
            stagger:1
        })

    })

</script>

    <nav >
        <ul> 
            <li class="listItems-nav"><a href="/">Hom</a></li>
            <li class="listItems-nav"><a href="/">About</a></li>
            <li class="listItems-nav"><a href="/">Contact</a></li>
        </ul>
    </nav>


<style>
    nav{
        background-color: rgb(243, 166, 243);
        height:15vh;

    }
    ul{
        display: flex;
        justify-content: space-around;
        align-items: center;
        height:15vh;

        
    }
    li{
        
        list-style-type: none;
        align-self: center;
    }
    li a{
        color: black;
        text-decoration: none;
        font-size: 1.5em;
        font-weight: 300;
    }
</style>