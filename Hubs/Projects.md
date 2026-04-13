## In flight:
```dataview
TABLE 
    without ID
	Title, 
	link(file.link, "here") as link,
	Status, 
	Target_End_Date as "End Date", 
	Owner
FROM 
	-"Templates" AND 
	#project
WHERE 
	Status="in-progress"
SORT 
	Due DESC
```

## Completed:
```dataview
TABLE 
    without ID
	title, 
	link(file.link, "here") as link,
	Target_End_Date as "End Date", 
	Owner
FROM 
	-"Templates" AND 
	#project
WHERE 
	Status="done"
SORT 
	Due DESC
```
