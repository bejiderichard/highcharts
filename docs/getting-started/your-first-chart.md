Highcharts.chart('container', {
    chart: {
        type: 'area'
    },
    title: {
        text: 'Unsafe Driving Habits',
        align: 'left'
    },
    yAxis: {
        title: {
            useHTML: true,
            text: 'Unsafe Driving Habits Event Count'
        }
    },
  

    tooltip: {
        shared: true,
        headerFormat: '<span style="font-size:12px"><b>{point.key}</b></span>' +
            '<br>'
    },
    plotOptions: {
        series: {
            pointStart: 2014
        },
        area: {
            stacking: 'normal',
            lineColor: '#666666',
            lineWidth: 1,
            marker: {
                lineWidth: 1,
                lineColor: '#666666'
            }
        }
    },
    series: [{
        name: 'Incidents',
        data: [
            434, 576, 472, 493, 328, 251,
            416, 504, 302, 379, 128
        ]
    }, {
        name: 'Speeding',
        data: [
            3502, 3844, 4139, 4351, 3802, 4020,
            4461, 5074, 4558, 3247, 3694
        ]

    }, {
        name: 'Harsh Driving',
        data: [
            2019, 2189, 2150, 2217, 2179, 2258,
            2348, 3196, 3018, 3180, 3127
        ]
}, {
        name: 'Risky Driving',
        data: [
            3502, 3844, 4139, 4351, 3802, 4020,
            4461, 5074, 3558, 4247, 5694
        ]

    }, {
         name: 'Distraction',
        data: [
            2019, 2189, 2150, 2217, 2179, 2258,
            2348, 2196, 3018, 3180, 3127
        ]   
    

    
    }]
});

