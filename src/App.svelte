<script>
  import Container from './Container.svelte';
  import Heading from './Heading.svelte';
  import Button from './Button.svelte';
  import Counter from './Counter.svelte';
  import Image from './Image.svelte';
</script>

<style>
  :global(:root){
    --pinkColor: salmon;
    --greyColor: lightgrey;
    --redColor: red;
  }
</style>

<Container>
  <Heading text="The Final Countdown-appen"/>
  <Button type="button" text="Räkna ner"/>
  <Counter />
  <Image src="jtempest.jpg"/>
</Container>
