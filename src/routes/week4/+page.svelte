<script>
    import {gsap} from 'gsap';
	import {ScrollTrigger} from "gsap/dist/ScrollTrigger";    
	import { onMount } from "svelte";
    onMount(() => {
        gsap.registerPlugin(ScrollTrigger)
        gsap.from('li:nth-child(1)', {
			scrollTrigger: {
                start: "top center",
                end: "top 100px",
				trigger: 'li:nth-child(1)',
				toggleActions:"restart none restart restart"
			},
            delay: 0,
			x:1000,
			opacity: 1,
			duration:2,
		});
        gsap.from('li:nth-child(2)', {
			scrollTrigger: {
				trigger: 'li:nth-child(2)',
                start: "top center",
				toggleActions:"restart none restart restart"
			},
            delay: 0,
			x:-1000,
			opacity: 1,
			duration:2,
		});

        gsap.from('li:nth-child(4)', {
			scrollTrigger: {
				trigger: 'li:nth-child(4)',
				toggleActions:"restart none restart restart"
			},
            delay: 0,
			x:1000,
			opacity: 1,
			duration:2,
		});
        gsap.from('li:nth-child(5)', {
			scrollTrigger: {
				trigger: 'li:nth-child(5)',
				toggleActions:"restart none restart restart"
			},
            delay: 0,
			x:-1000,
			opacity: 1,
			duration:2,
		});



    })
</script>
<section>
    <ul>
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
        <li>5</li>
    </ul>
</section>
<style>
    section{
        display: grid;
        place-items: center;
        overflow: hidden;
    }
    ul{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
    }
    li{
        display:grid;
        place-items: center;
        width: 10em;
        height: 10em;
        margin: 2em;
        background-color: darkmagenta;
        color: white;
    }
</style>