---
up: 
related: 
created: 2025-04-06
---
Take a look at this amazing dataview query for [[Records]].

```
TABLE WITHOUT ID
	choice(contains(file.path, "Calendar/Records/Events"), 
		"🎪 " + file.link,
	choice(contains(file.path, "Calendar/Records/Ideas"), 
		"💡 " + file.link,
	choice(contains(file.path, "Calendar/Records/Logs"), 
		"🪵 " + file.link,
	choice(contains(file.path, "Calendar/Records/Meetings"),
		"☎️ " + file.link,
	choice(contains(file.path, "Calendar/Records/Nice Things"),
		"🌈 " + file.link,
	file.link))))) as "Record",
    
    regexreplace(file.path, ".*/([^/]+)/[^/]+$", "$1") as "Parent Folder"

FROM "Calendar/Records"

WHERE 
    regextest("\\d{4}-\\d{2}-\\d{2}", file.name)

SORT regexreplace(file.name, ".*?(\\d{4}-\\d{2}-\\d{2}).*", "$1") DESC

LIMIT 35
```

If you don't want the emojis to be rendered, then use the following instead. This general adjustment can work for any dataview query where you want to remove the emojis:

```
TABLE WITHOUT ID
    file.link as "Record",
    regexreplace(file.path, ".*/([^/]+)/[^/]+$", "$1") as "Parent Folder"
    
FROM "Calendar/Records"

WHERE regextest("\\d{4}-\\d{2}-\\d{2}", file.name)

SORT regexreplace(file.name, ".*?(\\d{4}-\\d{2}-\\d{2}).*", "$1") DESC

LIMIT 44
```

