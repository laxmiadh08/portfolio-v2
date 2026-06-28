---
layout: default

permalink: /projects/price-transparency/
---
<style> 
.page-header{
    display:none;
}
.project-header { background-image: url("/images/price-transparency/dashboard-overview.png"); background-size: cover; background-position: center; 
height: 600px;

border-radius: 4px;
border:1px solid #ccc; 
width: 1120px;
margin-bottom: 25px; 
position: relative; }

.back-home { display: inline-block;
 margin: 10px 0; 
 padding: 10px 16px; 
 background: #FF7B00;
color: white; 
text-decoration: none; 
border-radius: 6px; 
font-weight: bold; } 


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
    font-size: 1.6rem;
    font-weight: 700;
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

<p class="project-title"> Price Transparency in Healthcare</p>

<p class="project-tech">
Power BI • Python • Data Modeling (Star Schema)
</p>

<p class="lead">
Analyzed negotiated rates, cash prices, and gross charges across three major hospitals in Louisville, Kentucky to uncover pricing disparities and support more informed healthcare decision-making.
</p>
<div class="project-header"></div>

<div class="project-highlight">
<p class="project-info">
Healthcare price transparency has been federally required since 2021, yet pricing files remain difficult for patients, insurers, and researchers to interpret. 
This project transforms raw hospital transparency data from UofL Health, Baptist Health, and Norton Hospital into an interactive analytics dashboard that makes pricing information accessible and actionable.
</p>
</div>

<p>

The original hospital pricing files contained 7,230,075 records combined for three hospitals. For this analysis, the data was narrowed to 49  high-impact healthcare procedures spanning inpatient, outpatient, emergency, laboratory, and pharmacy services, resulting in a curated dataset of approximately 6,681 records optimized for cross-hospital price comparisons.
</p>

</section>


<section>

<h3 class="text-bold">Business Questions</h3>
<ul>
<li>Which procedures have the highest negotiated rates?</li>
<li>How large is the difference between hospital gross charges and insurer negotiated rates?</li>
<li>How do negotiated prices vary across hospitals for the same procedure?</li>
<li>How do self-pay cash prices compare with negotiated insurance rates?</li>
</ul>

</section>


<section>

<b>Hospitals Included: </b>
<ul>
<li>UofL Health — Louisville, KY</li>
<li>Baptist Health — Louisville, KY</li>
<li>Norton Hospital — Louisville, KY</li>
</ul>

</section>


<section>



<p><b>Data Source: </b>
Data was collected from publicly available Hospital Price Transparency files released under the CMS Hospital Price Transparency Rule (45 CFR Part 180).
</p>

</section>





<section>

<h3 class="text-bold">Project Summary</h3>



<div class="metrics-grid">

<div class="metric-card">
    <p>Total Procedures Analyzed</p>
    <h3>48</h3>
</div>

<div class="metric-card">
    <p>Total Payers</p>
    <h3>46</h3>
</div>
<div class="metric-card">
    <p>Total Plans</p>
    <h3>53</h3>
</div>


<div class="metric-card">
    <p>Cash vs Min Negotiated Rate</p>
    <h3>$1.8K</h3>
</div>

<div class="metric-card">
    <p>Max Price Spread</p>
    <h3>$22.56K</h3>
</div>



</div>

<p class="insight">
The average gross charge is nearly <strong>four times</strong> higher than the average negotiated rate, illustrating the significant difference between published hospital prices and what insurers actually pay.
</p>

</section>


<section>

<h3 class="text-bold">Procedures Included</h3>

<div class="procedure-grid">

<ul>

</ul>

</div>

</section>


<section>

<h3 class="text-bold">Data Model</h3>

<img src="/images/price-transparency/data-model.png?raw=true"
     alt="Healthcare Price Data Model"
     class="project-image">

</section>


<section>



<div class="feature-card">

<h3 class="text-bold">Executive KPI Dashboard</h3>

<p>
Interactive KPI cards summarize the most important pricing metrics, including total procedures, participating payers, negotiated rates, cash prices, and gross hospital charges.
</p>

<pre><code>
Avg Negotiated Rate =
CALCULATE(
    AVERAGE('fact_prices'[negotiated_rate]),
    FILTER(
        fact_prices,
        NOT ISBLANK(fact_prices[negotiated_rate]) &&
        fact_prices[negotiated_rate] >= 50
    )
)
</code></pre>

<pre><code>
Median Negotiated Rate =
CALCULATE(
    MEDIAN('fact_prices'[negotiated_rate]),
    fact_prices[negotiated_rate] >= 50
)
</code></pre>

</div>

</section>


<section>

<h3 class="text-bold">Top 10 Most Expensive Procedures</h3>

<p>
Ranks procedures by average negotiated rate, clearly identifying Total Knee Replacement as the highest-cost procedure.
</p>

<img src="/images/price-transparency/top10.png?raw=true"
     alt="Top 10 Procedures"
     class="project-image">

</section>


<section>

<h3 class="text-bold">Negotiated Rate vs Cash Price</h3>

<p>
Compares negotiated insurance rates with cash prices across hospitals, showing that uninsured patients frequently pay substantially more than insurers.
</p>

<img src="/images/price-transparency/negotiated-vs-cash.png?raw=true"
     alt="Negotiated Rate vs Cash Price"
     class="project-image">

</section>


<section>

<h3 class="text-bold">Trans</h3>

<p>

</p>

<img src="/images/price-transparency/comparison.png?raw=true"
     alt="Hospital Comparison"
     class="project-image">

</section>


<section>

<h2>Key Insights</h2>

<div class="insight-card">

<h3 class="text-bold">Pricing Gap</h3>

<p>
Average gross charges ($30,794) are nearly four times higher than negotiated insurer payments ($7,740). Cash prices fall between these values, meaning uninsured patients often pay substantially more than insurance companies.
</p>

</div>

<div class="insight-card">

<h3 class="text-bold">Total Knee Replacement</h3>

<p>
Total Knee Replacement is a significant outlier and heavily influences average pricing. This explains why the median negotiated rate ($1,284) is much lower than the mean ($7,740).
</p>

</div>

<div class="insight-card">

<h3 class="text-bold">Norton Hospital Premium Pricing</h3>

<p>
Norton Hospital consistently reports higher negotiated rates for MRI Brain procedures, approaching five times the negotiated prices observed at UofL Health for the same services.
</p>

</div>

<div class="insight-card">

<h3 class="text-bold">Competitive Pricing</h3>

<p>
Across several common procedures—including CT Abdomen &amp; Pelvis and Colonoscopy—UofL Health generally reports the lowest negotiated rates, Baptist Health falls in the middle, and Norton Hospital reports the highest negotiated prices.
</p>

</div>

</section>















<!-- ## Screenshots

![Dashboard](/assets/images/env-dashboard.png) -->

---

### Back to Home
[← Return Home](/)