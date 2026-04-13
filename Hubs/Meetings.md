```dataview
TABLE
  without ID
  file.link as link,
  Date,
  join(Attendees, ", ") as "Who"
FROM 
	-"Templates" and
	#meeting
SORT 
	Date DESC
```
