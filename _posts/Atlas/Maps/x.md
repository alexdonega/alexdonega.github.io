---
up: 
related: 
created: 2025-04-09 10:19
---
~ [[Home Pro]] 
 
> [!ghost] **[[x]]** » [[Packs]] | [[x/Templates/Templates]] | [[Visuals]] 

"x" stands for "extras." That's how it got its name. It convenient sorts near the bottom of any folder, exactly where extra things should be. But that's not to diminish anything in "x". It might sort to the bottom, but it's not at the bottom of our hearts. 

Below are the notes in the **x** folder, sorted by recently modified. 

```dataview
TABLE WITHOUT ID
	choice(contains(file.path, "x/Packs"),
		"🎒 " + file.link,
	choice(contains(file.path, "x/Templates"),
		"📋 " + file.link,
	choice(contains(file.path, "x/Visuals"),
		"🖼️ " + file.link,
	choice(contains(file.path, "x/x"),
		"𝔁 " + file.link,
	file.link)))) as "Notes in x",

 (date(today) - file.mday).day as "Days ago"

FROM "x"

WHERE
	!contains(file.name, "Template")

SORT file.mtime desc

LIMIT 55
```

---


Back to [[Home Pro]] 
