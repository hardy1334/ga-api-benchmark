# ga-api-benchmark (on-going project)

## Purpose
This project was conducted to establish industry benchmarks within plastic & cosmetic surgery, medical spas, and addiction treatment centers. The secondary purpose of this project is to use the aggregated data to analyze the effects of numerous Google Search Algorithm Upates occurring throughout 2019. This is an ongoing project that has not yet been completed.

### Data Source
<img src="https://user-images.githubusercontent.com/31733278/70547741-695dfb80-1b97-11ea-978d-4aa20991b982.jpg" alt="google analytics" />
- The data was acquried from multiple Google Analytics accounts utilizing the [Google Analytics API](https://developers.google.com/analytics/devguides/reporting/core/v4/).

<p>The Google Analytics Reporting API v4 is the most advanced programmatic method to access report data in Google Analytics. With the Google Analytics Reporting API, you can:</p>
<ul>
    <li>Build custom dashboards to display Google Analytics data.</li>
<li>Automate complex reporting tasks to save time.</li>
<li>Integrate your Google Analytics data with other business applications.</li>
</ul>

### Relational Database
-  [SQLite](https://www.sqlite.org/index.html) is used as Database

### Python Libraries
- Primary Python libraries used include pandas, matplotlib, NumPy, datetime, and os
<br/>
    <b>Pandas</b><p><a href="https://pandas.pydata.org/">Pandas</a> is an open source, BSD-licensed library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming language.Pandas is a NumFOCUS sponsored project. This will help ensure the success of development of pandas as a world-class open-source project, and makes it possible to donate to the project.</p>
   <b>Matplotlib</b>
   <p><a href="https://matplotlib.org/">Matplotlib</a>is a Python 2D plotting library which produces publication quality figures in a variety of hardcopy formats and interactive environments across platforms. Matplotlib can be used in Python scripts, the Python and IPython shells, the Jupyter notebook, web application servers, and four graphical user interface toolkits.</p>
   <b>Numpy</b><p><a href="https://numpy.org/">Numpy</a>is the fundamental package for scientific computing with Python. It contains among other things:
<ul>
    <li>a powerful N-dimensional array object</li>

<li>sophisticated (broadcasting) functions</li>

<li>tools for integrating C/C++ and Fortran code</li>

<li>useful linear algebra, Fourier transform, and random number capabilities</li>
</ul>
Besides its obvious scientific uses, NumPy can also be used as an efficient multi-dimensional container of generic data. Arbitrary data-types can be defined. This allows NumPy to seamlessly and speedily integrate with a wide variety of databases.

NumPy is licensed under the BSD license, enabling reuse with few restrictions.</p>


## How to Access and Utilize the Google Analytics API
-   [Enabling the API](https://console.developers.google.com/start/api?id=analyticsreporting.googleapis.com&credential=client_key)

<img src="https://user-images.githubusercontent.com/31733278/70550164-5cdba200-1b9b-11ea-8972-226b2ea30baf.jpg" alt="analytics" />
   <ul> <li>  Creating a project in the Google API Console</li>
    <li>   Enabling the API</li>
    <li>  Creating credentials (cred.json)</li></ul>
    
## How to Get This Project Running Locally 
-   After following the setup guide for [Google Analytics API using Python](https://developers.google.com/analytics/devguides/reporting/core/v4/quickstart/service-py) you will need to grant read and analyze access to the email address on the Google Analytics accounts you want to pull data from. This email should be provided to you by Google
-   Add the view id of every Google Analytics account you want to pull data from into the config.py file
-   Run main.py, which will pull Google Analytics data into the SQLite database and then into a CSV file in the sheets folder
-   Open ga-api-benchmark.ipynb using Jupyter Notebook and run the cells which will manipulate the data and plot it according to the analysis conducted
## Benefits Google Analytics API vs Google Analytics Native  
-   Aggregating data across multiple clients to create industry benchmarks
    -   Ability to compare individual clients to benchmark to assess performance
    -   Analyzing effects of Google Algorithm update
-   Better data visualization with more flexiblity
    -   Better internal reporting for Account Managers and Search Engine Optimization Specialists to use when creating client strategies
    -   Publishing of industry data analysis
-   Combine metrics to get more insight
    -   For example: goal completions per number of sessions
