<script>
  // import {setContext} from 'svelte';

  import Label from './Label.svelte';
  import Input from './Input.svelte';
  import Button from './Button.svelte';

  export let asdf = 'bajs';
  // setContext('message', {success: 'The form has been sent.'});
</script>

<form>
  <Label text="Name" forId="name"/>
  <Input id="name" bind:value={asdf}/>

  <Button type="button" text="Register"/>
  {asdf}
</form>
