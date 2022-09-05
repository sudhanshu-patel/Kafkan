---
tags: 
alias: Home
cssClasses: cards cards-1-1 table-wide
---
# Dashboard

Managed by Sudhanshu Patel
Open source project to share and solve community problems.

## Goals
```dataview
TABLE WITHOUT ID
	(link(file.path, alias)) as title,
	Bar
FROM #goal
WHERE Progress != Target
SORT Type DESC
```

## Projects
```dataview
TABLE WITHOUT ID
	(link(file.path, alias[0])) as title,
	subtitle,
	("Goal: " + link(Goal, Goal.alias)) as goal
FROM #project
WHERE status = "In Progress"
```
