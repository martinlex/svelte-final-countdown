<script>
  import { count } from './stores.js';

  export let type;
  export let text;

  let countValue;

  const unsubscribe = count.subscribe(value => {
    countValue = value;
  });

  const decrement = () => {
    if (countValue !== 0) count.update(n => n - 1);
  };
</script>

<style>
  button {
    background-color: var(--pinkColor);
    border: 2px solid var(--pinkColor);
    color: #fff;
  }
  button[disabled] {
    background-color: var(--greyColor);
    border: 2px solid var(--greyColor);
  }
</style>

<button type={type} on:click={decrement} disabled='{countValue === 0}'>{text}</button>
