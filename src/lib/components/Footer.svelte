<script>
  import gsap from 'gsap';
  import { onMount } from "svelte";
  onMount(() => {
    gsap.to("footer", { duration: 8, x: 0, delay: "3", ease: "elastic" });
    gsap.from(".listItemsfoot", {
      duration: 1.5,
      opacity: 0,
      delay: "1.5",
      stagger: 1,
    });
  });
</script>

<footer>
  <ul>
    <li class="listItemsfoot"><a href="/">Home</a></li>
    <li class="listItemsfoot"><a href="/">About</a></li>
    <li class="listItemsfoot"><a href="/">Contact</a></li>
    <li class="listItemsfoot"><a href="/">E-mal</a></li>
  </ul>
</footer>

<style>
  footer {
    transform: translateX(100%);
    background-color: rgb(7, 79, 211);
    height: 15vh;
  }
  ul {
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 15vh;
  }
  li {
    list-style-type: none;
    align-self: center;
  }
  li a {
    color: rgb(245, 237, 237);
    text-decoration: none;
    font-size: 1.5em;
    font-weight: 300;
  }
</style>
