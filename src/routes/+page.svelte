<script>
  import ButtonLayers from "$lib/components/ButtonLayers.svelte";
  import ButtonCircle from "$lib/components/ButtonCircle.svelte";
  import ButtonFolds from "$lib/components/ButtonFolds.svelte";
  import ButtonOpening from "$lib/components/ButtonOpening.svelte";
  import ButtonSwap from "$lib/components/ButtonSwap.svelte";
  import ButtonWave from "$lib/components/ButtonWave.svelte";

  let test = "Yo Dawg";
</script>

<div class="container">
  <!-- <ButtonLayers />
  <ButtonCircle />
  <ButtonFolds />
  <ButtonOpening />
  <ButtonSwap {test} /> -->
  <ButtonWave />
</div>

<style>
  .container {
    display: flex;
    flex-direction: column;
  }
</style>
