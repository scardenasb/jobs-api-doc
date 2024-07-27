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
<code>https://avgjobs.top</code>
<br>
<br>
<h4>ENDPOINTS</h4>
<h4>Main</h4>
<b>GET</b>
<b>/jobs</b>
<p>Returns a JSON object containing all the jobs (there can be a large amount of data).</p>
<div>
<code>{"jobs": [{"country": "Brazil", "jobs": 49000, "new_jobs": -49000, "date": "2024-07-20"}, {"country": "Canada", "jobs": 23000, "new_jobs": -23000, "date": "2024-07-20"}, {"country": "Chile", "jobs": 3000, "new_jobs": -3000, "date": "2024-07-20"}, {"country": "China", "jobs": 131000, "new_jobs": -131000, "date": "2024-07-20"}, {"country": "Denmark", "jobs": 2000, "new_jobs": -2000, "date": "2024-07-20"}, {"country": "Estonia", "jobs": 74, "new_jobs": -74, "date": "2024-07-20"}, {"country": "Finland", "jobs": 1000, "new_jobs": -1000, "date": "2024-07-20"}], "status_code": 200}</code>
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
<code>{"jobs": [{"country": "Japan", "jobs": 42000, "new_jobs": -42000, "date": "2024-07-20"}, {"country": "Japan", "jobs": 43000, "new_jobs": 1000, "date": "2024-07-21"}, {"country": "Japan", "jobs": 41000, "new_jobs": -2000, "date": "2024-07-22"}], "status_code": 200}</code>
</div>
<br>
<h4>Dates as endpoints</h4>
<b>GET</b>
<b>/jobs/2024-07-20</b><br>
<p>Returns every record on the given date.</p>
<div>
<code>{"jobs": [{"country": "Brazil", "jobs": 49000, "new_jobs": -49000, "date": "2024-07-20"}, {"country": "Canada", "jobs": 23000, "new_jobs": -23000, "date": "2024-07-20"}, {"country": "Chile", "jobs": 3000, "new_jobs": -3000, "date": "2024-07-20"}, {"country": "China", "jobs": 131000, "new_jobs": -131000, "date": "2024-07-20"}, {"country": "Denmark", "jobs": 2000, "new_jobs": -2000, "date": "2024-07-20"}, {"country": "Estonia", "jobs": 74, "new_jobs": -74, "date": "2024-07-20"}, {"country": "Finland", "jobs": 1000, "new_jobs": -1000, "date": "2024-07-20"}, {"country": "France", "jobs": 65000, "new_jobs": -65000, "date": "2024-07-20"}, {"country": "Germany", "jobs": 108000, "new_jobs": -108000, "date": "2024-07-20"}], "status_code": 200}</code>
</div>
</div>
</section>
<br/>
<br/>
<br/>
<p>This API is for informational purposes only and is provided free of charge. I am not responsible for any decisions made based on the provided information.</p>
<br/>
</body>
