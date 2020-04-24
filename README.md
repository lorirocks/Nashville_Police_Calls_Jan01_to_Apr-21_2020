# Nashville_Police_Calls_Jan_to_Apr_2020
Tableau project #2 for Nashville Software School

<p>Police calls from Saturday Jan 1st to Tuesday April 14th 2020<br>
Rows:  234014<br>
Columns: 23 (in cleaned database)<br>
</p>
<p>Data Cleaning Notes:<br>
The original database included dates from Wed. Jan. 1, 2020 through Tuesday April 14, 2020. In Excel, I created a new, cleaned dataset as follows:<br></p>
<p>1. The "Call Received" column contained the date (MM/DD/YYYY) and the time. I split that into four columns:  Date, Time, Day of Week, and Week Number (with Week 1 starting on Saturday, Jan. 4th). I chose these dates so that I could get full weeks, starting on Saturdays and ending on Fridays.  After extracting the information, I saved each column at "Value"<br>
     Code used to extract date:  =INT(B2)<br>
     Code use to extract time: =MOD(B2,1)<br>
     Code used to identify day of week:  =CHOOSE(WEEKDAY(C2),"Sun","Mon","Tue","Wed","Thu","Fri","Sat")<br>
     Code used to identify week number, with weeks starting on Mondays* (Mon-Sun):  =WEEKNUM(C2,2)<br>
     * Weeks were ended on Sunday so that the entire weekend (Fri-Sat-Sun) was counted within one week)<br></p>
 
     


