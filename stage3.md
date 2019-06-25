# Consolidated Logs
Click the Test Plan
Right click the Test Plan > add > Listener > View Results Tree

We can now rename the HTTP Requests so we can tell the difference
Click on the first HTTP Sampler 
Change the name to HTTP Sampler 2

Repeat with the second HTTP Sampler, calling this one HTTP Sampler 2
Now run and view the results tree to ensure that they have the correct names


## Variables
Click on the Test Plan. Click Add under the User Defined Variables section.

| Name       | Value            |
|------------|------------------|
| servername | crawler-test.com |

Format for variables: ${servername}

## Add to Sampler
Click on the first HTTP Sampler.

Change the website name to ${servername}

## Clear Results

We can clear existing results to clean up. The icon for this is two brooms over a cog wheel. 


## Multi Threading
Click the first Thread Group to view its properties. 
Change the following:
Number of threads: 5 
Ramp-up period: 10


Run again
Check the results

# Summary Report
JMeter – different types of listener
Right click Test Plan  > Add > Listener > Summary report 

Click the play button to run the tests again

This will show different rows for each “Label”


# Graphical Report
Right click Test Plan > Add > Listener > Graph Results 

Once you run the test plan now, you can look at the graph results listener

Graphs might not be solid due to bottlenecks and load 

