<script context="module">
  export async function preload(page) {
    return { state: page.params["state"] };
  }
</script>

<script>
  import CovidStat from "../components/CovidStat.svelte";
  import CovidChart from "../components/CovidChart.svelte";
  import TableContainer from "../components/TableContainer.svelte";

  export let state;
</script>

<h2>{state}</h2>

<CovidStat />
<CovidChart />
