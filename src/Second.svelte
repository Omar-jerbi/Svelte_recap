<script>
  import {MDCRipple} from '@material/ripple';
  import { onMount } from 'svelte';

  onMount(()=>{
    const buttonRipple = new MDCRipple(document.querySelector('.mdc-button'));
  });
</script>

<style global lang="scss">
  @use "@material/button/styles";
  @use "src/scss/Second.scss";//IMPORTANT METTI CARTELLA SCSS SOTTO SRC
</style>


<button class="mdc-button mdc-button--raised mdc-button--leading">
  <span class="mdc-button__ripple"></span>
  <i class="material-icons mdc-button__icon" aria-hidden="true"
    >O</i
  >
  <span class="mdc-button__label"><a id="lollo" href="index.html"> vai a index</a></span>
</button>


