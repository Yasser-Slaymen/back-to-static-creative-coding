<div class="App-container">
  <main class="carousel__container">
    <frame class="carousel__content">
      <div class="caixa__card cc__1">PROGRAMADOR <br /> CS</div>
      <div class="caixa__card cc__2">HTML</div>
      <div class="caixa__card cc__3">CSS</div>
      <div class="caixa__card cc__4">JS</div>
      <div class="caixa__card cc__5">GIT</div>
      <div class="caixa__card cc__6">REACT</div>
      <div class="caixa__card cc__7">Node.js</div>
      <div class="caixa__card cc__8">sveltekit</div>
    </frame>
  </main>
</div>

<style>
  * {
    font-family: "Verdana", sans-serif;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
    letter-spacing: 0px;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    scroll-behavior: smooth;
    margin: 0;
    color: #fff;
  }

  .App-container {
    display: grid;
    place-items: center;
    height: 68vh;
  }
  .carousel__container {
    display: grid;
    place-items: center;
   
  }
  .carousel__content {
    display: grid;
    place-items: center;
    -webkit-perspective: 250px;
    -moz-perspective: 250px;
    perspective: 250px;
    width: 400px;
    height: 200px;
    /* background-color: #1472ff; */
  }

  @keyframes efeitoCarrosel {
    from {
      -webkit-transform: rotateY(360deg) translateZ(130px) rotateY(-360deg);
      -moz-transform: rotateY(360deg) translateZ(130px) rotateY(-360deg);
      z-index: 10;
      opacity: 1;
    }

    50% {
      z-index: -10;
    }

    to {
      -webkit-transform: rotateY(0deg) translateZ(130px) rotateY(0deg);
      -moz-transform: rotateY(0deg) translateZ(130px) rotateY(0deg);
      z-index: 10;
      opacity: 1;
    }
  }

  @-moz-keyframes efeitoCarrosel {
    from {
      -moz-transform: rotateY(360deg) translateZ(130px) rotateY(-360deg);
      z-index: 10;
      opacity: 1;
    }

    50% {
      z-index: -10;
    }

    to {
      -moz-transform: rotateY(0deg) translateZ(130px) rotateY(0deg);
      z-index: 10;
      opacity: 1;
    }
  }

  .caixa__card {
    width: 100px;
    height: 142px;
    background-color: #442222;
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
    top:40px;
    left:150px;
    font-size: 9px;
    border-radius: 8px;
    box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.5);
    text-align: center;
    -webkit-animation-name: efeitoCarrosel;
    animation-name: efeitoCarrosel;
    -moz-animation-name: efeitoCarrosel;
    -webkit-animation-duration: 8s;
    -moz-animation-duration: 8s;
    animation-duration: 8s;
    -webkit-animation-iteration-count: infinite;
    animation-iteration-count: infinite;
    -moz-animation-iteration-count: infinite;
    -webkit-animation-timing-function: linear;
    animation-timing-function: linear;
    -moz-animation-timing-function: linear;
    
  }

  .caixa__card:hover {
    border: solid #4466cc 3px;
    box-shadow: 0px 0px 10px #4466cc;
  }

  .caixa__card.cc__1 {
    background: linear-gradient(-229deg, #0093e9, #80d0c7);
    -webkit-animation-delay: -7s;
    animation-delay: -7s;
    -moz-animation-delay: -7s;
  }

  .caixa__card.cc__2 {
    background: linear-gradient(-229deg, #00dbde, #fc00ff);
    -webkit-animation-delay: -6s;
    animation-delay: -6s;
    -moz-animation-delay: -6s;
  }

  .caixa__card.cc__3 {
    background: linear-gradient(-229deg, #50d990, #d4d054);
    -webkit-animation-delay: -5s;
    animation-delay: -5s;
    -moz-animation-delay: -5s;
  }

  .caixa__card.cc__4 {
    background: linear-gradient(-229deg, #cf91ff, #5782f5);
    -webkit-animation-delay: -4s;
    animation-delay: -4s;
    -moz-animation-delay: -4s;
  }

  .caixa__card.cc__5 {
    background: linear-gradient(-229deg, #642b73, #c6426e);
    -webkit-animation-delay: -3s;
    animation-delay: -3s;
    -moz-animation-delay: -3s;
  }

  .caixa__card.cc__6 {
    background: linear-gradient(-229deg, #d9afd9, #97d9e1);
    -webkit-animation-delay: -2s;
    animation-delay: -2s;
    -moz-animation-delay: -2s;
  }

  .caixa__card.cc__7 {
    background: linear-gradient(-229deg, #fbab7e, #f7ce68);
    -webkit-animation-delay: -1s;
    animation-delay: -1s;
    -moz-animation-delay: -1s;
  }

  .caixa__card.cc__8 {
    background: linear-gradient(-229deg, #1472ff, #a8eb12);
  }
</style>
