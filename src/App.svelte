<script>
  import { onMount } from "svelte";//IMPORTANT
  import {MDCRipple} from '@material/ripple';

  export let name;

  onMount(()=>{//IMPORTANT
    const buttonRipple = new MDCRipple(document.querySelector('.mdc-button'));
  });
</script>

<style global lang="scss">//IMPORTANT
  @use "@material/button/styles";

  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>

<main>
  <h1>Hello {name}!</h1>
  <p>Main Svelte-Page</p>
</main>


<button class="mdc-button">
  <span class="mdc-button__ripple"></span>
  <span class="mdc-button__label">Text Button</span>
</button>

<a href="second.html"> vai a 2</a>

