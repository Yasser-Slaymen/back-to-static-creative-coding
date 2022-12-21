<section class="box">
    <a href="/">Home</a>
</section>
<style>
   .box{
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    width: 200px;
    height: 200px;
    box-shadow: 16px 14px 20px black;
    border-radius: 10px;
    overflow: hidden;
    margin-bottom: 2em;
   }
   a{
    display: grid;
    place-items: center;
    align-items: center;
    text-align: center;
    text-decoration: none;
    font-size: 1.5em;
    width: 200px;
    height: 200px;
    z-index: 999;
    color: #ff0052;
   }
   .box::before{
    content:"";
    background-image: conic-gradient(#ff0052 20deg, transparent 120deg);
    width: 150%;
    height: 150%;
    position: absolute;
    animation: rotate 2s linear infinite;
   }
   .box::after{
    content: "";
    display: flex;
    justify-content: center;
    align-items: center;
    width: 190px;
    height: 190px;
    background-color: black;
    position: absolute;
    border-radius: 10px;
    color: #ff0052;
    font-size: large;
    box-shadow: inset 20px 20px 20px #0000008c;
   }
   @keyframes rotate {
    0%{
        transform: rotate(0deg); 
    }
    100%{
        transform: rotate(-360deg);
      
    }
   }
   

</style>