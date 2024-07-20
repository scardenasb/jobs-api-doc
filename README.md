# Api to get current and new Python jobs

### Table of Content

* [Documentation](#documentation)
* [Base Url](#base-url)
* [Endpoints](#endpoints)

<br></br>
## Documentation
Api to get data from a DB, which contains average Python jobs info published on the Web,
this data is related to the following countries and contains info since 2022-06-29.

- Brazil
- Canada
- Chile
- China
- Denmark
- Estonia
- Finland
- France
- Germany
- India
- Ireland
- Italy
- Japan
- Luxembourg
- Netherlands
- Portugal
- Scotland, United Kingdom
- South Korea
- Spain
- Sweden
- Switzerland
- Taiwan
- United Kingdom
- United States
<br></br>
## Base Url
```
https://injobsapi.herokuapp.com/api
```
<br></br>
## Endpoints
**GET** ```/jobs```

It returns a JSON object containing all the jobs (there can be a large amount of data).

```
{"jobs": [{"id": 1, "jobs": 22000, "country": "Japan", "new_jobs": 389, "date": "2022-06-29"}, {"id": 2, "jobs": 43000, "country": "Netherlands", "new_jobs": 2155, "date": "2022-06-29"}, {"id": 3, "jobs": 434334, "country": "Japan", "new_jobs": 3499, "date": "2022-06-30"}]}
```

### **Supported Query Filters**
> **Country** or **Date**


**GET** ```/jobs/Japan```

It returns all the data related to that country.

```
{"jobs": [{"id": 1, "jobs": 22000, "country": "Japan", "new_jobs": 389, "date": "2022-06-29"}, {"id": 3, "jobs": 434334, "country": "Japan", "new_jobs": 3499, "date": "2022-06-30"}]}
```
<br></br>
**GET** ```/jobs/2022-06-29```

Returns every record on the given date.

```
{"jobs": [{"id": 1, "jobs": 22000, "country": "Japan", "new_jobs": 389, "date": "2022-06-29"}, {"id": 2, "jobs": 43000, "country": "Netherlands", "new_jobs": 2155, "date": "2022-06-29"}]}
```
