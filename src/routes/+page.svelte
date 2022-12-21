<main>
	<div>
	  <h1 class="headerHome">Creative Coding</h1>
	  <ul>
		<li><a href="/week1">Week1-loading</a></li>
		<li><a href="/week2">Week2-Circular effect</a></li>
		<li><a href="/week3">Week3-Cards animation</a></li>
	  </ul>
	</div>
  </main>
  
  <style>
	main {
	  display: grid;
	  place-items: center;
	  width: 100vw;
	  height: 100vh;
	  background-color:black;
	}
	div {
	  display: grid;
	  grid-row: auto;
	  place-items: center;
	  grid-gap: 7em;
	  height: 50vh;
	  width: 50vw;
	}
	.headerHome{
	  color: whitesmoke;
	}
	ul {
	  display: flex;
	  justify-content:space-around;
	  gap: 4em;
	  width: 100%;
	  list-style: none;
	}
	li {
	  position: relative;
	  display: flex;
	  justify-content: center;
	  align-items: center;
	  width: 15em;
	  height: 4em;
	  background-color:#FFE3F1;
	  border-radius: 0.5em;
	  transition: ease-out 0.3s;
	  outline: none;
	  z-index: 1;
	}
	a {
	  text-align: center;
	  text-decoration: none;
	  color:black;
	  font-size: 1.5rem;	
	  font-weight: 500;
	}
	li::before{
	  content: "";
	  transition:0.6s all ease;
	  position: absolute;
	  top: 0;
	  left: 50%;
	  right: 50%;
	  bottom: 0;
	  opacity: 0;
	  background-color:#00AAA9;
	  border-radius: 0.5em;
	}
  
	li:hover::before{
	  transition: 0.5s all ease;
	  left: 0;
	  right: 0;
	  opacity: 1;
	  z-index: -1;
  
	}
	a:hover{
	  color:whitesmoke;
	  cursor: pointer;
	} 
  </style>
  
