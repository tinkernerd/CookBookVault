---
title: Recipes
created_at: 2024-11-20T14:50:00
type: Dashboard/L1
category: Recipes
---

# `= this.title`
## Drinks
```dataview  
TABLE WITHOUT ID  
link(file.path, title) AS "Note", drinktype AS "Alcohol?", file.mtime AS "Last modified"
WHERE contains(category, "Recipes") AND contains(topic, "Drinks")
SORT title ASC
```
## Food  
```dataview  
TABLE WITHOUT ID  
link(file.path, title) AS "Note", file.mtime AS "Last modified"
WHERE contains(category, "Recipes") AND contains(topic, "Food")
SORT title ASC
```
