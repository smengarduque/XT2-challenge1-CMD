var ctx = document.getElementById('myChart').getContext('2d');
var chart = new Chart(ctx, {
    // The type of chart we want to create
    type: 'line',

    // The data for our dataset
    data: {
        labels: ['January', 'February', 'March', 'April', 'May', 'June', 'July'],
        datasets: [{
            label: 'Massa',
            backgroundColor: 'rgb(255, 99, 132)',
            borderColor: 'rgb(255, 99, 132)',
            data: [0, 10, 5, 2, 20, 30, 45]
        }]
    },

    // Configuration options go here
    options: {}
});

/*PEI CHART*/
/*const CHART = document.getElementById('linechart');
Chart.default.scale.ticks.beginAtZero=true;

let barChart = new Chart(CHART,{
    type: 'pie'
    data: {
        labels: ['Water','Voedsel'],
        datasets:[
        {
            label: 'points',
            backgroundcolor:['#64F9FF','#C8FDFD'
            data: [60,40]
            }
        ]
    }
});*/

google.charts.load('current', {'packages':['corechart']});
google.charts.setOnLoadCallback(drawChart);

      function drawChart() {

        var data = google.visualization.arrayToDataTable([
          ['Task', 'Hours per Day'],
          ['Eten',     11],
          ['Water',      6],
        ]);

        var options = {
          title: ''
        };

        var chart = new google.visualization.PieChart(document.getElementById('piechart'));

        chart.draw(data, options);
      }

/*Area Chart*/

    google.charts.load('current', {'packages':['corechart']});
    google.charts.setOnLoadCallback(areaChart);

      function areaChart() {
        var data = google.visualization.arrayToDataTable([
          ['kilometer', 'Brandstof', 'Temperatuur'],
          ['10.000',  1000,      1400],
          ['20.000',  1170,      1120],
          ['30.000',  660,       1000],
          ['40.000',  1030,      800],
          ['50.000',  660,       600],
          ['60.000',  660,       540]
        ]);

        var options = {
          title: '',
          hAxis: {title: 'Kilometers',  titleTextStyle: {color: '#333'}},
          vAxis: {minValue: 0}
        };

        var chart = new google.visualization.AreaChart(document.getElementById('areaChart'));
        chart.draw(data, options);
      }