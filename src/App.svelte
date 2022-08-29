<script lang="ts">
  import DiscSelection from "./lib/DiscSelection.svelte";
  import Greet from "./lib/Greet.svelte";
</script>

<main class="container">
  <div class="fill">
    <DiscSelection />
  </div>
</main>

<style>
.container {
  margin: 0;
  padding: 0;
  width: 100vw;
  height: 100vh;
}

.fill {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
}
</style>
