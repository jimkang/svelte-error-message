<script>

export let error;
</script>

{#if error}
  <div class="error-message">
    <div>{error.message}</div>
    <pre>{error.stack}</pre>
  </div>
{/if}
