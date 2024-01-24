<h1>Applying filters to SQL queries</h1>

<h2>Project Description</h2>
In this project, I will demonstrate basic SQL filters to help the given company with security related issues like checking suspicious log entries and providing information for device update requests.
<br />


<h2>Language Used</h2>

- <b>SQL</b> 

<h2>Retrieve after hours failed login attempts:</h2>

<p align="center">
In this task there was a potential security incident after 18:00. The request was that I investigate all failed login attempts made after that time.
The following code demonstrates the SQL query I made to investigate the logs: <br/>
<img src="https://i.imgur.com/VM2MKIM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <p align="center">
  First I selected all data from the log_in_attempts table.
After that I used the WHERE clause and the AND operator to filter my results on failed login attempts that occurred after 18:00.
‘success = 0’ refers to failed login attempts and bracket between login_time and 18:00 means to filter before that time.
<br />
<br />
<h2>Retrieve login attempts on specific dates:</h2>

   <p align="center">
    A suspicious login attempt was made on the date: 2022-05-09. The request was that I investigate all login activity that day, including the day before.
The following code demonstrates the SQL query made to investigate the logs on the given days.
<img src="https://i.imgur.com/r2iQbvh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p align="center">
First I selected all data from the log_in_attempts_table.
After that I used the WHERE clause and the OR operator to filter my output to only the date 2022-05-08 and 2022-05-09.  <br/>
<br />
<br />
  <h2>Retrieve login attempts outside of Mexico:</h2>
  <p align="center">
In this task I was told that suspicious login activity was detected and also that it’s certain that it’s outside of Mexico.
The following code demonstrates the SQL query I made to filter the login attempts outside of mexico. <br/>
<img src="https://i.imgur.com/vGsKbZW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <p align="center">
  First I selected all data from the log_in_attempts table.
After that I used the WHERE clause and NOT operator to filter out login attempts outside of mexico. I also used the LIKE operator with ‘Mex%’ to filter out every data starting with Mex.
The % represents, in this case, that any amount and type of character can be after the word ‘mex’.
<br />
<br />
    <h2>Retrieve employees in Marketing:</h2>
    <p align="center">
In this task there was an update request for certain computers. I had to provide information about the desired devices.
This SQL query demonstrates the code I made to filter out the devices.  <br/>
<img src="https://i.imgur.com/d8ItZXd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <p align="center">
    First I selected all data from the employees table.
After that I used the WHERE clause with AND to filter out every type of East offices at the Marketing department.
The “office LIKE ‘East%’ ” line represents this.
<br />
<br />
      <h2>Retrieve employees in Finance or Sales:</h2>
      <p align="center">
The devices from the Sales and Marketing department also needed an update.
Since this was a different kind of security update, I had to filter out only these two departments
The following SQL query demonstrates the code I used for this task.  <br/>
<img src="https://i.imgur.com/YxU7F53.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
       <p align="center">
      TFirst I selected all employees from the employees table.
After that I used the WHERE clause with OR to filter out employees in the Finance and Sales department.
I used OR instead of AND because I want the list of all employees working in those two departments.
<br />
<br />
<h2>Retrieve all employees not in IT:</h2>
           <p align="center">
In this task, a security update was also requested, this time it was everyone excluding the IT department.
The following SQL query demonstrates the code I made to filter this out.  <br/>
<img src="https://i.imgur.com/UPUHRb7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
           <p align="center">
           First I selected all employees from the employees table.
After that I used the WHERE clause and the NOT operator to filter out every department outside of the IT department.
<h2>Summary</h2>
In this project I applied different types of filters to SQL queries to help me get specific kinds of information from the database.
I used two different kinds of tables to draw information from.
I also used AND, OR, NOT, operators to help me get specific information.
On top of that I used LIKE and the (%) wildcard to help me filter for patterns.
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
