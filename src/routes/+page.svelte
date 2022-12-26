<script>
  import ButtonLayers from "$lib/components/ButtonLayers.svelte";
  import ButtonCircle from "$lib/components/ButtonCircle.svelte";
  import ButtonFolds from "$lib/components/ButtonFolds.svelte";
  import ButtonOpening from "$lib/components/ButtonOpening.svelte";
  import ButtonSwap from "$lib/components/ButtonSwap.svelte";
  import ButtonWave from "$lib/components/ButtonWave.svelte";
  import LightningText from "$lib/components/LightningText.svelte";
  import AnimatedText from "$lib/components/AnimatedText.svelte";
  import Ping from "$lib/components/Ping.svelte";
  import LoadingSplit from "$lib/components/LoadingSplit.svelte";

  let test = "Yo Dawg";
</script>

<div class="container">
  <h2>Buttons</h2>
  <ButtonLayers />
  <ButtonCircle />
  <ButtonFolds />
  <ButtonOpening />
  <ButtonSwap {test} />
  <ButtonWave />
  <Ping />
  <h2>Animated Text</h2>
  <LightningText />
  <AnimatedText />

  <h2>Loading Animations</h2>
  <LoadingSplit />
</div>

<style>
  .container {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  h2 {
    font-size: 3rem;
    margin: 0;
    text-align: center;
  }
</style>
