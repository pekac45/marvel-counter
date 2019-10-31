<script>
  import Counter from "./Counter.svelte";
</script>

<style>
  .page {
    background: #333;
  }
</style>

<page class="page" actionBarHidden="true">
  <actionBar title="DMG" icon="" flat="true" />
  <Counter />
</page>
