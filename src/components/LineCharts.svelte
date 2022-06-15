<script>
  import Line from "svelte-chartjs/src/Line.svelte";

  const options = {
    responsive: true,
    scales: {
      yAxes: {
        id: "y-axis-1",
        type: "linear",
        position: "right",
        grid: {
          display: false,
        },
      },
    },
  };

  let data = {
    labels: ["January", "February", "March", "April", "May", "June", "July"],
    datasets: [
      {
        label: "My First dataset",
        backgroundColor: "rgb(45,164,78)",
        borderColor: "rgb(45,164,78)",
        data: [65, 59, 80, 81, 56, 55, 40],
        yAxisID: "y-axis-1",
      },
      {
        label: "My Second dataset",
        backgroundColor: "rgb(207,34,46)",
        borderColor: "rgb(207,34,46)",
        data: [28, 48, 40, 19, 86, 27, 90],
        yAxisID: "y-axis-1",
      },
    ],
  };
</script>

<Line {data} {options} />
