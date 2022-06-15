<script>
  import LineCharts from "./components/LineCharts.svelte";
  import PieCharts from "./components/PieCharts.svelte";
</script>

<main>
  <h2>Line Charts</h2>
  <LineCharts />

  <h2>Pie Charts</h2>
  <PieCharts />
</main>

<style>
  main {
    margin-left: auto;
    margin-right: auto;
    width: 30%;
    height: 30%;
  }

  h2 {
    text-align: center;
  }
</style>
