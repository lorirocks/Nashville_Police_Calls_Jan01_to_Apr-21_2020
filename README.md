# Nashville_Police_Calls_Jan_to_Apr_2020 - Tableau Assignment

DESCRIPTION: We started learning Tableau on Monday 4/20/2020 in the data analytics course in Nashville Software School. This was one of our first assignments.  

ASSIGNMENT:  Find our own data from a public source, develop a scenerio and question to query the data, and make a brief presentation.  

TIMELINE from start to finish:  1.5 days   

LINK TO FINAL PROJECT:  https://public.tableau.com/profile/loributler#!/vizhome/pub_metro_police_calls_jan_to_apr_2020/TornadosImpactonPoliceCalls?publish=yes

DATA SOURCE:  https://data.nashville.gov/Police/Metro-Nashville-Police-Department-Calls-for-Servic/nhhg-pnxf


DESCRIPTION AND NOTES:  
Police calls from Saturday Jan 1st to Tuesday April 14th 2020
Rows:  234014
Columns: 22 (in cleaned database)

Data Cleaning Notes:
The original database included dates from Wed. Jan. 1, 2020 through Tuesday April 14, 2020. I created a new, cleaned dataset in Excel, as follows:  
1. The "Call Received" column contained a datetime field. I split that into four columns:  Date, Time, Day of Week, and Week Number (with Week 1 starting on Saturday, Jan. 4th. I chose these dates so that I could get full weeks, starting on Saturdays and ending on Fridays.  After extracting the information, I saved each column at "Value"
* Code used to extract date:  =INT(B2)  
* Code use to extract time: =MOD(B2,1)  
* Code used to identify day of week:  =CHOOSE(WEEKDAY(C2),"Sun","Mon","Tue","Wed","Thu","Fri","Sat")  
     


