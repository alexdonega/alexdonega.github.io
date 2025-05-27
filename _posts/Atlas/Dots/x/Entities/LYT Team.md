---
collection:
  - "[[Entities]]"
related: 
created: 2024-07-20
---
 ~ [[Entities]] 

The Linking Your Thinking team. 

---

All notes in `Calendar` linking to `LYT Team`
```dataview
TABLE WITHOUT ID
file.link as Meeting,
one-liner as One-liner

FROM "Calendar"

WHERE contains(file.name,this.file.name)

SORT file.name desc
```

---

This shows all meeting notes where the `meetingGroups` property is set to `LYT Team`. 

This will also show any notes in the "Calendar" folder where you have a line that starts with `meeting::` and then includes the title of this note: `LYT Team`.
```dataview
LIST

FROM "Calendar"

WHERE contains(meetingGroups, this.file.link) OR contains(meeting, this.file.name) 

SORT file.name desc
```
