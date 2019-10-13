<script>
  export let forId;
  export let text;
</script>

<style>
  label {
    color: var(--greyColor);
    margin-bottom: var(--spacingUnit);
  }
</style>

<label for={forId}>{text}</label>
