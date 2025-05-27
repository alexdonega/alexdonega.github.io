---
up:
  - "[[Atlas]]"
collection:
  - "[[Maps]]"
  - "[[Views]]"
related: 
created: 2025-04-01
---
~ [[Atlas]] 

> [!shapes] [[Things]] | [[Statements]] | [[People]] | [[Quotes]] | [[Questions]] 

Dots are **any bit of knowledge**. Connecting the dots often leads to meaningful leaps of insights, creative breakthroughs, and valuable contributions. You might think of dots as concepts, or quotes, but they also include any "thing" and even "statements about things". Below are the most recently created notes in the **Dots** folder.
```dataview
TABLE WITHOUT ID
	choice(contains(file.path, "Atlas/Dots/Things"), 
		"🧩 " + file.link,
	choice(contains(file.path, "Atlas/Dots/Statements"), 
		"📣 " + file.link,
	choice(contains(file.path, "Atlas/Dots/People"), 
		"👤 " + file.link,
	choice(contains(file.path, "Atlas/Dots/Quotes"),
		"💬 " + file.link,
	choice(contains(file.path, "Atlas/Dots/Questions"),
		"❓ " + file.link,
	choice(contains(file.path, "Atlas/Dots/x"),
		"𝔁 " + file.link,
	file.link)))))) as "Dots",
    
    regexreplace(file.path, ".*/([^/]+)/[^/]+$", "$1") as "Parent Folder",

	length(file.inlinks) as "Links"

FROM "Atlas/Dots"

SORT file.ctime desc

LIMIT 77
```

---

Additional dots include: [[Questions]], PKM, and Entities.

---


Back to [[Atlas]] 