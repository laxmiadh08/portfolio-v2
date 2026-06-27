---
layout: default

permalink: /projects/cdc/
---
<style> 
.page-header{
    display:none;
}
.project-header { background-image: url("/images/cdc/overview.jpg"); background-size: cover; background-position: center; 
height: 400px;
width:100%;
border-radius: 4px;
border:1px solid #ccc;
margin: 25px 0; 
position: relative; } 
.back-home { display: inline-block; margin: 20px 0; padding: 10px 16px;  background: #FF7B00;
color: #ffffff;text-decoration: none; border-radius: 6px; font-weight: bold; }

.metrics-grid {
    display: grid;
    gap: 16px;
    margin: 2rem 0;
    grid-auto-flow: column
}

.metric-card {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap:wrap;
    padding: 18px 24px;

    background: #ffffff;
    border: 1px solid #e5e7eb;
    border-radius: 10px;

    transition: all .2s ease;
}

/* .metric-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 18px rgba(0,0,0,.08);
} */

.metric-card p {
    margin: 0;
    font-size: 0.95rem;
    color: #555;
    font-weight: 500;
}

.metric-card h3 {
    margin: 0;
    font-size: 1rem;
    font-weight: 600;
    color: #0f172a;
    white-space: nowrap;
}
.project-title{
    font-weight:900;
    font-size:36px;
    margin:8px 0 !important;
}
.project-tech{
    margin:4px 0px!important;
}
.project-info{
    font-size:16px;
    font-style:italic;
    opacity:0.85;
}
.text-bold{
    font-weight:bold!important;
}

</style>


<a class="back-home" href="/">← Back to Home</a>


<section class="project-content">

<h1 >Ischemic Heart Disease Mortality in Kentucky (2019–2024)</h1>

<p class="project-tech">
Public Health Analytics • CDC WONDER • Excel • Datawrapper
</p>

<p class="lead">
Analyzed county-level ischemic heart disease mortality across all 120 Kentucky counties to identify geographic disparities and highlight high-burden regions for targeted public health intervention.
</p>

<div class="project-highlight">
<p>
Heart disease remains the leading cause of death in the United States. Although Kentucky consistently ranks among the states with the highest cardiovascular mortality, substantial variation exists within the state. Rural Appalachian counties experience mortality rates more than twice the national average, while several urban and suburban counties report rates well below both state and national benchmarks.
</p>
</div>

</section>

<section>
<img src="/images/cdc/comparision.png?raw=true"
  alt="Kentucky vs National Comparison"
  class="project-image">
<h3 class="text-bold">Executive Summary</h3>

<p>
Using CDC WONDER mortality data from 2019–2024, this analysis evaluated crude ischemic heart disease mortality rates across every Kentucky county. The project identifies geographic clusters of elevated mortality and compares county performance against state and national benchmarks.
</p>

<div class="metrics-grid">

<div class="metric-card">
<p>Counties Analyzed</p>
<h3>120</h3>
</div>

<div class="metric-card">
<p>Highest Mortality Rate</p>
<h3>375</h3>
</div>

<div class="metric-card">
<p>Kentucky Mean</p>
<h3>165</h3>
</div>

<div class="metric-card">
<p>National Mean</p>
<h3>145</h3>
</div>

<div class="metric-card">
<p>Highest Burden County</p>
<h3>Breathitt</h3>
</div>

<div class="metric-card">
<p>Study Period</p>
<h3>2019–2024</h3>
</div>

</div>

<div class="metrics-grid">

<div class="metric-card">
<p>Cause of Death</p>
<h3>I20–I25</h3>
</div>

<div class="metric-card">
<p>Geography</p>
<h3>120 KY Counties</h3>
</div>

<div class="metric-card">
<p>Time Period</p>
<h3>2019–2024</h3>
</div>

<div class="metric-card">
<p>Rate Type</p>
<h3>Crude Rate</h3>
</div>

<div class="metric-card">
<p>Population</p>
<h3>All Residents</h3>
</div>

</div>

</section>

<section>

<h3 class="text-bold">Key Findings</h3>

<ul>
<li>Breathitt County recorded the highest crude mortality rate in Kentucky at approximately <strong>375 deaths per 100,000</strong>, more than 2.5 times the national average.</li>

<li>The ten highest-burden counties are concentrated almost entirely within Eastern Kentucky's Appalachian region.</li>

<li>Kentucky's statewide mortality rate (<strong>165 per 100,000</strong>) exceeds the national average (<strong>145 per 100,000</strong>) by approximately 14%.</li>

<li>The lowest-burden counties, including Shelby and Madison, reported mortality rates near 35–40 per 100,000—nearly ten times lower than the highest-burden counties.</li>

<li>The statewide choropleth map reveals a clear east-to-west mortality gradient, with eastern counties consistently experiencing the greatest disease burden.</li>

</ul>

</section>

<section>

<p class="text-bold">Data Source</p>

<p>
Mortality data was obtained from the CDC WONDER online database using county-level mortality records for ischemic heart disease (2019 -2024)
</p>


</section>

<section>

<h3>Tools Used</h3>

<ul>
<li><strong>CDC WONDER</strong> — Mortality data extraction</li>
<li><strong>Microsoft Excel</strong> — Data cleaning, aggregation, and statistical summaries</li>
<li><strong>Datawrapper</strong> — Interactive choropleth map visualization</li>
</ul>

<div class="project-highlight">
<p>
<strong>Note:</strong> CDC WONDER suppresses county-level values with fewer than ten deaths to protect patient privacy. Suppressed counties were excluded from ranking analyses.
</p>
</div>

</section>

<section>

<h3 class="text-bold">Geographic Distribution</h3>
<img src="/images/cdc/map.png?raw=true"
  alt="Kentucky Heart Disease Choropleth Map"
  class="project-image">

<p>
The county-level choropleth map reveals a pronounced geographic concentration of heart disease mortality.
</p>

<ul>

<li><strong>Eastern Kentucky (Appalachia)</strong> shows the highest mortality rates, with counties such as Breathitt, Perry, Bell, Wolfe, and Whitley approaching or exceeding 300–375 deaths per 100,000.</li>

<li><strong>Central Kentucky</strong> exhibits moderate mortality levels that generally align with the statewide average.</li>

<li><strong>Western Kentucky</strong> displays mixed results, with isolated high-burden counties but overall lower mortality than Eastern Kentucky.</li>

<li><strong>Urban and suburban counties</strong>, including Jefferson (Louisville), Fayette (Lexington), Shelby, and Madison, consistently report the lowest mortality rates.</li>

</ul>

</section>

<section>

<h3 class="text-bold">Top 10 Highest-Burden Counties</h3>

<p>
The ranking below highlights the counties with the highest ischemic heart disease mortality rates during the study period.
</p>

<img src="/images/cdc/top10.png?raw=true"
  alt="Top 10 Highest Burden Counties"
  class="project-image">

</section>


<!-- <h2>State and National Benchmark Comparison</h2> -->

<!-- <p>
County mortality rates were compared against Kentucky and national averages to quantify the magnitude of regional disparities.
</p> -->

<!-- <img src="/images/cdc/comparision.png?raw=true"
  alt="Kentucky vs National Comparison"
  class="project-image"> -->



<section>

<h3 class="text-bold">Key Insights</h3>

<div class="insight-card">

<h3 class="text-bold">Regional Health Inequality</h3>

<p>
The mortality difference between the highest- and lowest-performing counties spans approximately <strong>338 deaths per 100,000</strong>, representing one of the largest county-level health disparities within Kentucky.
</p>

</div>

<div class="insight-card">

<h3 class="text-bold">Appalachian Disease Burden</h3>

<p>
Eastern Kentucky counties consistently experience the highest mortality rates, suggesting that geographic, socioeconomic, and healthcare access factors contribute to a concentrated regional burden of cardiovascular disease.
</p>

</div>

<div class="insight-card">

<h3 class="text-bold">Statewide Performance</h3>

<p>
Kentucky's average mortality rate exceeds the national benchmark by roughly 14%, indicating that cardiovascular disease remains a statewide public health priority.
</p>

</div>

<div class="insight-card">

<h3 class="text-bold">Targeted Public Health Opportunities</h3>

<p>
The analysis demonstrates that statewide averages conceal substantial county-level variation. Prioritizing prevention and intervention efforts in high-burden Appalachian counties could produce the greatest public health impact.
</p>

</div>

</section>


<!-- ## Screenshots

![Dashboard](/assets/images/env-dashboard.png) -->

---

## Back to Home
[← Return Home](/)