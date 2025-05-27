---
collection:
  - "[[Collections]]"
  - "[[Maps]]"
related: 
created: 2022-01-01
rank: 1.5
mapState:
  - 🟩
---
~ [[Sources]]

> [!kindling] [[Books]] | [[Movies]] | [[Series]] | **[[Cursos]]** 

Se uma nota tiver a propriedade `collection` com o valor `Cursos`, ela será exibida abaixo.*

Cursos organizados por **YearXP** (ano de experiência):

```dataview
TABLE WITHOUT ID
	yearXP as YearXP,
	file.link as Title,
	join(list(by)) as By
WHERE
	contains(collection,this.file.link) and
	!contains(file.name, "Template")
SORT yearXP desc
```


---

Back to [[Sources]] 