<script type="ts">
  import Connect, { marinaStore, MarinaStore } from 'svelte-marina-button';

  // You can subscribe to marina status changes
  marinaStore.subscribe((s: MarinaStore) => {
    console.log(`Marina is attached to the ${s.network} network`);
  });
</script>

<div class="container is-widescreen">
  <div class="box">
    <h1 class="title">Hello fren!</h1>
    <Connect cssClass={'button'} />
  </div>
</div>

<style src="./scss/main.scss" lang="scss" global>
</style>
