<script>
  import { count } from './stores.js';

  let countValue;

  const unsubscribe = count.subscribe(value => {
    countValue = value;
  });
</script>

<style>
  .warning {
    color: var(--redColor);
  }
</style>

<p class:warning="{countValue < 4}">{countValue}</p>
