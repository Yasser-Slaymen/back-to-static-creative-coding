<script>
    import {gsap} from 'gsap';
	import { onMount } from "svelte";
    onMount(() => {
        
         gsap.from('.card', { duration:2, opacity: 0, delay: 1,
            stagger:1
        })

    })
</script>
<div class="App">
    <section class="container">
        <frame class="card">
            <section class="face face1">
                <div class="content">
                 <h3>windows</h3>
                </div> 
            </section>
            <section class="face face2">
                <div class="content">
                    <p>
                        Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                         Deserunt quidem vero accusantium alias illum expedita commodi 
                         animi, dolorem, aspernatur cum voluptatibus consequuntur porro, 
                     <p/>
                </div> 
            </section>
        </frame>
        <frame class="card">
            <section class="face face1">
                <div class="content">
                 <h3>Apple</h3>
                </div> 
            </section>
            <section class="face face2">
                <div class="content">
                    <p>
                        Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                         Deserunt quidem vero accusantium alias illum expedita commodi 
                         animi, dolorem, aspernatur cum voluptatibus consequuntur porro, 
                        
                    </p>
                </div> 
            </section>
        </frame>
        <frame class="card">
            <section class="face face1">
                <div class="content">
                 <h3>Android</h3>
                </div> 
            </section>
            <section class="face face2">
                <div class="content">
                    <p>
                        Lorem, ipsum dolor sit amet consectetur adipisicing elit.
                         Deserunt quidem vero accusantium alias illum expedita commodi 
                         animi, dolorem, aspernatur cum voluptatibus consequuntur porro, 
                         
                    </p>
                </div> 
            </section>
        </frame>
       
    </section>
</div>
<style>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        scroll-behavior: smooth;
    }
    .App{
        display: flex;
        justify-content: center;
        align-items: center;
        font-family: Arial, Helvetica, sans-serif;
        width: 100vw;
        min-height: 50vh;
        background-color: rgb(9, 18, 81);
    }
    .container{
        position: relative;
        display: flex;
        justify-content:space-around;
        align-items: center;
        flex-wrap: wrap;
        width: 1000px;
    }
    .container .card{
        position: relative;
    }
    .container .card .face{
        width: 300px;
        height: 200px;
        transition: ease-out .4s;
    }
    .face1{
        display: flex;
        justify-content: center;
        align-content: center;
        align-items: center;
        position: relative;
        z-index: 1;
        background-color: #333;
        transform: translateY(100px);
        cursor: pointer;
    }
    .card:hover .face1{
        transform: translateY(0);
        box-shadow:
        inset 0 0 60px whitesmoke,
        inset 20px 0 80px #f0f,
        inset -20px 0 80px #f0f,
        inset 20px 0 300px #f0f,
        inset -20px 0 300px #f0f,
        0 0 50px #f0f,
        -10px 0 80px #f0f,
        10px 0 80px #f0f;
    }
    .content{
        opacity: .1;
        transition: 0.5s;
        text-align: center;
    }
    .card:hover .content{
        opacity: 1;
    }
    h3{
        font-size: 1em;
        color:white;
        text-align: center;
    }
    .face2{
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 20px;
        box-shadow: 0 20px 50px rgba(0,0,0,.8);
        position: relative;
        background-color: whitesmoke;
        transform: translateY(-100px);
    }
    .card:hover .face2{
        transform: translateY(0);
    }
    .content p{
        font-size: 10pt;
        margin: 0;
        padding: 0;
        color: #333;
    }
</style>