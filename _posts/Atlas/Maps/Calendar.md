---
up:
  - "[[Home Pro Basic]]"
collection:
  - "[[Views]]"
  - "[[Maps]]"
related:
  - "[[Define your time-style]]"
down:
  - "[[Logs]]"
  - "[[Plan and Review]]"
created: 2023-08-19
rank: 1
---
~ [[Home Pro]] 

> [!calendar] [[Days]] | [[Records]] | [[Reviews]] 

Below is your amazing Calendar Activity Log (CAL) below. It compiles any note in all Calendar subfolders if it has a name with the date like `YYYY-MM-DD`.

```dataview
TABLE WITHOUT ID
    choice(contains(file.path, "/Days/"), 
        "— " + file.link,
	choice(contains(file.path, "Calendar/Records/Events/"), 
		"🎪 " + file.link,
	choice(contains(file.path, "Calendar/Records/Ideas"), 
		"💡 " + file.link,
	choice(contains(file.path, "Calendar/Records/Logs"), 
		"🪵 " + file.link,
	choice(contains(file.path, "Calendar/Records/Meetings"),
		"☎️ " + file.link,
	choice(contains(file.path, "Calendar/Records/Nice Things"),
		"🌈 " + file.link,
	choice(contains(file.path, "Calendar/Reviews"),
		"🔍 " + file.link,
	file.link))))))) as "Calendar Note",
    
    regexreplace(file.path, ".*/([^/]+)/[^/]+$", "$1") as "Parent Folder"

FROM "Calendar"

WHERE 
    regextest("\\d{4}-\\d{2}-\\d{2}", file.name) 

SORT regexreplace(file.name, ".*?(\\d{4}-\\d{2}-\\d{2}).*", "$1") DESC

LIMIT 77
```

---


If you use emojis in your filenames, like I do, then you'll want to use this dataview for the Calendar Activity Log (CAL). It won't magically render emojis to the front of some of the records.

```
TABLE WITHOUT ID
    choice(
        contains(file.path, "/Days/"), 
        "— " + file.link, 
        file.link
    ) as "Record",
    regexreplace(file.path, ".*/([^/]+)/[^/]+$", "$1") as "Parent Folder"
FROM "Calendar"
WHERE regextest("\\d{4}-\\d{2}-\\d{2}", file.name)
SORT regexreplace(file.name, ".*?(\\d{4}-\\d{2}-\\d{2}).*", "$1") DESC
LIMIT 35
```





