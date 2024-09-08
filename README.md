<body>
<header>
<h1>
Api to get Average IT jobs
</h1>
</header>
    <section>
        <div>
            <h2>WHAT IS THIS?</h2>
            <p>
                Data collected from major job websites, provides an <strong>average</strong> of the total number of jobs found.
            </p>
            <p>
                The 'new_jobs' key represents the delta between <strong>today jobs - yesterday jobs</strong>
            </p>
            <p>Current IT jobs provided by this api:</p>
            <ul>
                <li>Python</li>
                <li>Golang</li>
                <li>Flask</li>
                <li>Machine Learning</li>
                <li>Artificial Intelligence (AI)</li>
            </ul>
            <br/>
            <br/>
            <h2>HOW TO USE IT?</h2>
            <p>
                Just call an endpoint with <b>GET</b> http method.
            </p>
            <h4>BASE URL</h4>
            <p>
                Using v1 api as an example, look <a href="#changelog">here</a> for different versions (in case there are).
            </p>
            <code><a href="https://avgjobs.top/api/v1">https://avgjobs.top/api/v1</a></code>
            <br/>
            <br/>
            <h4>ENDPOINTS</h4>
            <h4>Main</h4>
            <b>GET</b>
            <b>/jobs</b>
            <p>Returns a JSON object containing all the jobs (there can be a large amount of data).</p>
            <div id="jobs">
                <code>{"jobs": [{"keyword": "Python", "country": "Brazil", "jobs": 49000, "new_jobs": -49000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Canada", "jobs": 23000, "new_jobs": -23000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Chile", "jobs": 3000, "new_jobs": -3000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "China", "jobs": 131000, "new_jobs": -131000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Denmark", "jobs": 2000, "new_jobs": -2000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Estonia", "jobs": 74, "new_jobs": -74, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Finland", "jobs": 1000, "new_jobs": -1000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "France", "jobs": 65000, "new_jobs": -65000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Germany", "jobs": 108000, "new_jobs": -108000, "date": "2024-07-20"}],
                    "status_code": 200}
                </code>
            </div>
            <br/>
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
                <li>Scotland</li>
                <li>South Korea</li>
                <li>Spain</li>
                <li>Sweden</li>
                <li>Switzerland</li>
                <li>Taiwan</li>
                <li>United Kingdom</li>
                <li>United States</li>
            </ul>
            <br/>
            <b>GET</b>
            <b>/jobs/unitedkingdom</b>
            <br>
            <p>It returns all the data related to that country.</p>
            <div id="jobs">
                <code>{"jobs": [{"keyword": "Python", "country": "United Kingdom", "jobs": 83000, "new_jobs": 83000, "date": "2024-08-10"},
                    {"keyword": "Golang", "country": "United Kingdom", "jobs": 85, "new_jobs": 85, "date": "2024-08-10"},
                    {"keyword": "Python", "country": "United Kingdom", "jobs": 94000, "new_jobs": -94000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "United Kingdom", "jobs": 96000, "new_jobs": 2000, "date": "2024-07-21"},
                    {"keyword": "Python", "country": "United Kingdom", "jobs": 92000, "new_jobs": -4000, "date": "2024-07-22"}],
                    "status_code": 200}
                </code>
            </div>
            <br>
            <h4>Dates as endpoints</h4>
            <b>GET</b>
            <b>/jobs/2024-07-20</b>
            <br>
            <p>Returns every record on the given date.</p>
            <div id="jobs">
                <code>{"jobs": [{"keyword": "Python", "country": "Brazil", "jobs": 49000, "new_jobs": -49000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Canada", "jobs": 23000, "new_jobs": -23000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Chile", "jobs": 3000, "new_jobs": -3000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "China", "jobs": 131000, "new_jobs": -131000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Denmark", "jobs": 2000, "new_jobs": -2000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Estonia", "jobs": 74, "new_jobs": -74, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Finland", "jobs": 1000, "new_jobs": -1000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "France", "jobs": 65000, "new_jobs": -65000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Germany", "jobs": 108000, "new_jobs": -108000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "India", "jobs": 123000, "new_jobs": -123000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Ireland", "jobs": 4000, "new_jobs": -4000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Italy", "jobs": 17000, "new_jobs": -17000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Japan", "jobs": 42000, "new_jobs": -42000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Luxembourg", "jobs": 1000, "new_jobs": -1000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Netherlands", "jobs": 43000, "new_jobs": -43000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Portugal", "jobs": 8000, "new_jobs": -8000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Scotland, United Kingdom", "jobs": 4000, "new_jobs": -4000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "South Korea", "jobs": 1000, "new_jobs": -1000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Spain", "jobs": 16000, "new_jobs": -16000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Sweden", "jobs": 8000, "new_jobs": -8000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Switzerland", "jobs": 11000, "new_jobs": -11000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "Taiwan", "jobs": 3000, "new_jobs": -3000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "United Kingdom", "jobs": 94000, "new_jobs": -94000, "date": "2024-07-20"},
                    {"keyword": "Python", "country": "United States", "jobs": 342000, "new_jobs": -342000, "date": "2024-07-20"}],
                    "status_code": 200}
                </code>
            </div>
        </div>
    </section>
<p>This API is for informational purposes only and is provided free of charge. I am not responsible for any decisions made based on the provided information.</p>
</body>
