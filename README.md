<body>
<header>
<h1>
Api to get Average Python jobs
</h1>
</header>
<section>
<div>
<h3>WHAT IS THIS?</h3>
<p>Data collected from major job sites on the internet, provides an <strong>average</strong> of the total number of jobs found.</p>
<p>The 'new_jobs' key represents the delta between <strong>today jobs - yesterday jobs</strong></p>
<br>
<br>
<h3>HOW TO USE IT?</h3>
<p>Just call an endpoint with <b>GET</b> http method.</p>
<h4>BASE URL</h4>
  
  [https://jobs-avg.up.railway.app](https://jobs-avg.up.railway.app)
<br/>
<br/>
<h4>ENDPOINTS</h4>
<h4>Main</h4>
<b>GET</b>
<b>/jobs</b>
<p>Returns a JSON object containing all the jobs (there can be a large amount of data).</p>
<div>
<code>{"jobs": [{"id": 1, "jobs": 22000, "country": "Japan", "new_jobs": 389, "date": "2022-06-29"}, {"id": 2, "jobs": 43000, "country": "Netherlands", "new_jobs": 2155, "date": "2022-06-29"}, {"id": 3, "jobs": 434334, "country": "Japan", "new_jobs": 3499, "date": "2022-06-30"}]}</code>
</div>
<br>
<h4>Countries as endpoint</h4>
<p>Countries with data at the moment</p>
<ul>
<li>Brazil</li>
<li>Canada</li>
<li>Chile</li>
<li>China</li>
<li>Denmark</li>
<li>Estonia</li>
<li>Finland</li>
<li>France</li>
<li>Germany</li>
<li>India</li>
<li>Ireland</li>
<li>Italy</li>
<li>Japan</li>
<li>Luxembourg</li>
<li>Netherlands</li>
<li>Portugal</li>
<li>Scotland, United Kingdom</li>
<li>South Korea</li>
<li>Spain</li>
<li>Sweden</li>
<li>Switzerland</li>
<li>Taiwan</li>
<li>United Kingdom</li>
<li>United States</li>
</ul>
<br>
<b>GET</b>
<b>/jobs/Japan</b><br>
<p>It returns all the data related to that country.</p>
<div>
<code>{"jobs": [{"id": 1, "jobs": 22000, "country": "Japan", "new_jobs": 389, "date": "2022-06-29"}, {"id": 3, "jobs": 434334, "country": "Japan", "new_jobs": 3499, "date": "2022-06-30"}]}</code>
</div>
<br>
<h4>Dates as endpoints</h4>
<b>GET</b>
<b>/jobs/2022-06-29</b><br>
<p>Returns every record on the given date.</p>
<div>
<code>{"jobs": [{"id": 1, "jobs": 22000, "country": "Japan", "new_jobs": 389, "date": "2022-06-29"}, {"id": 2, "jobs": 43000, "country": "Netherlands", "new_jobs": 2155, "date": "2022-06-29"}]}</code>
</div>
</div>
</section>
</body>
