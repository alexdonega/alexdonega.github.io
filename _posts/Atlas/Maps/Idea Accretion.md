---
up:
  - "[[Home Pro]]"
collection:
  - "[[Maps]]"
  - "[[Views]]"
related: 
created: 2023-10-15
rank: 1.5
mapState:
  - 🟩
---
~ [[Add]] 

Never start with a blank page. Surprise yourself with the work you've invisibly done already.

This very advanced view shows accreting placeholder notes with at least `3` links pointing to it If you get the spark, turn the placeholder note into an actual note.

```dataviewjs
const count = 3;
let d = {};
function process(k, v) {
  Object.keys(v).forEach(function (x) {
    x = dv.fileLink(x);
    if (d[x]==undefined) { d[x] = []; }
    d[x].push(dv.fileLink(k));
  });
}

Object.entries(dv.app.metadataCache.unresolvedLinks)
    .filter(([k,v])=>Object.keys(v).length)
    .forEach(([k,v]) => process(k, v));
    
dv.table(["Accreting placeholder notes", "Linked from"],
         Object.entries(d)
         .filter(([k, v]) => v.length >= count)
         .sort((a, b) => b[1].length - a[1].length)
         .map(([k,v])=> [k, v.join(" • ")]))
```
 
 You can also think of these as: shadow seeds, secret slowburns, accreting placeholder notes.

---

Go to [[Add]] 
