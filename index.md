---
layout: home
title: Tests for Interactive Graphs
subtitle: OMG, Graphs Are Interactive! 
---

<div class="main-content">
    <p>Let's try to make this graph interactive</p>
    <br>

    <!-- Interactive Graph Placeholder -->
    <div id="degree-distribution" style="width: 100%; height: 500px;"></div>
    <br>

    <!-- Description -->
    <p>
        This graph represents the degree distribution of our dataset. Hover over the points to see detailed values or zoom in for a closer look!
    </p>
</div>

<!-- Include Plotly.js Library -->
<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>

<!-- Add Script for Rendering the Graph -->
<script>
    var data = [
        {
            x: [0, 1, 2, 3, 4, 5],  // Replace with actual degree values
            y: [5, 15, 10, 7, 3, 1], // Replace with actual frequency values
            type: 'bar',
            marker: {
                color: 'darkblue'
            }
        }
    ];

    var layout = {
        title: 'Degree Distribution',
        xaxis: { title: 'Degree' },
        yaxis: { title: 'Frequency' },
        paper_bgcolor: '#f9f9f9',
        plot_bgcolor: '#ffffff'
    };

    // Render the Plotly graph
    Plotly.newPlot('degree-distribution', data, layout);
</script>


