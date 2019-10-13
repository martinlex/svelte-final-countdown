<script>
  import { count } from './stores.js';

  export let src;

  let countValue;

  const unsubscribe = count.subscribe(value => {
    countValue = value;
  });
</script>

{#if countValue === 0}
  <img {src}/>
{/if}
