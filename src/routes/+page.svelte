<script>
  import ButtonLayers from "$lib/components/ButtonLayers.svelte";
  import ButtonCircle from "$lib/components/ButtonCircle.svelte";
  import ButtonFolds from "$lib/components/ButtonFolds.svelte";
  import ButtonOpening from "$lib/components/ButtonOpening.svelte";
  import ButtonSwap from "$lib/components/ButtonSwap.svelte";

  let test = "Hover Me";
</script>

<div class="container">
  <ButtonLayers />
  <ButtonCircle />
  <ButtonFolds />
  <ButtonOpening {test} />
  <ButtonSwap {test} />
</div>

<style>
  .container {
    display: flex;
    flex-direction: column;
  }
</style>
