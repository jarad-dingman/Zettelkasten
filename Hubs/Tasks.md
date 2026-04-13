## Upcoming:

```dataview
TASK
FROM "Content" OR "Daily"
WHERE !completed
AND due >= date(today)
SORT due ASC, file.name ASC
```
## Missing Due Date:

```dataview
TASK
FROM "Content" OR "Daily"
WHERE !completed
AND due = null
SORT file.name ASC, line ASC
```

### Completed:
```dataview
TASK
WHERE completed
GROUP BY completion
SORT completion DESC
```