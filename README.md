# JMeter
================

Referred: Raghav pals youtube crash course JMeter

Mac How to run tests from command line.

-n -> non GUI mode

-t -> Test plant

-l -> to store Results -> results.jtl  sh jmeter -n -t "/Users/sriramku/Desktop/jmeter/Counter.jmx"  -l "report1.csv"


Results can be generated in 2 formats 
1) csv
2) jtl -> we can use this file to generate reports using some external tools


Monitor results using Blazemeter cloud

Go to https://a.blazemeter.com/app/#/accounts/1257239/workspaces/1292491/dashboard

Create test & upload jmx file of the Jmeter test

and click Run it will run and gives the result

https://a.blazemeter.com/app/#/accounts/1257239/workspaces/1292491/projects/1544420/masters/64026219/summary 


To check help

sh jmeter.sh -h


To Run & generate html report

sh jmeter -n -t "/Users/sriramku/Desktop/jmeter/ReportExample.jmx"  -l "results.csv" -e -o "html_reports"

To just generate html report from existing results file

sh jmeter -g  -l "results.csv" -e -o "html_reports"

