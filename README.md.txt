📘 Power Apps DTR (Daily Time Record) App

A Power Apps solution for automating employee attendance tracking.
This app allows employees to Clock In, Lunch Out, Lunch In, and Clock Out with one tap — recording timestamps automatically to a connected SharePoint list.

🧩 Features

✅ Simple One-Tap Logging
Each button (Clock In, Lunch Out, Lunch In, Clock Out) updates both:

The EmployeeTbl (main record with current status)

The Employee_Log (detailed time log for every action)

✅ Real-Time Status Updates
The app automatically updates the employee’s current status (e.g., “Clocked In”, “Lunch Out”, etc.) in the SharePoint table.

✅ Secure Access
Each user is matched to their record using their Microsoft 365 email, ensuring accurate logging.

✅ Timezone Adjusted
All times are saved with an 8-hour offset (Philippines Standard Time / UTC+8).

🗂 SharePoint Lists
1. EmployeeTbl

Stores current status and timestamps for each employee.

Column Name	Type	Description
Employee Name	Text	Full name of the employee
Email	Text	User’s Microsoft 365 email
NormalizedEmail	Text	Lowercase version of email for matching
Status - A	Choice/Text	Current status (Clock In, Lunch Out, etc.)
ClockInTime	DateTime	Time of clock-in
LunchOutTime	DateTime	Time of lunch-out
LunchInTime	DateTime	Time of lunch-in
ClockOutTime	DateTime	Time of clock-out