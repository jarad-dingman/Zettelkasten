---
Mood:
---
## Notes Created:
```dataview
TABLE file.ctime AS "Created", file.mtime AS "Modified"
FROM "Content"
WHERE file.cday = this.file.day OR file.mday = this.file.day
SORT file.mtime DESC
```

### Due Today:

```dataview
TASK
FROM "Content" OR "Daily"
WHERE !completed
AND due = date(this.file.name)
SORT file.name ASC, due ASC
```

### Todays Theme and Actions:

One short sentence that defines the day.

- **Theme:** 
- **Top priority:**

### Meetings:

- links to meetings...

### Events / Incidents / Changes:

Anything noteworthy that affects systems, projects, or people.

- **Event:**  
	- Description:  
	- Impact:  
	- Links:

## Notes:

Anything extra to add?

### End-of-day Review

- [ ] Did I finish my top priority?  
- [ ] One thing I’m grateful for: