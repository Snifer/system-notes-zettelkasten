---
cssclass: academia, academia-rounded, cards, dashboard
banner: "https://data.whicdn.com/images/220738162/original.gif"
banner_icon: 📖
banner_y: 0.516
Status: 
---
# Articles
- [[Library/Videos/000 Library|🗄️ Library]]
- [[000 Books|📚 Books]]
- [[000 Articles|📖 Articles]]
- [[000 Courses|📚 Courses]]
- [[000 Videos|📹 Videos]]
---

```button
name New Register
type command
action QuickAdd: Library
```


---

```dataview
TABLE without id 
  ("![cover|90](" + Cover + ")") as Cover,
  file.link AS "Title",
  Author AS "Author",
  Type, 
  Status

 
FROM "Library/Articles"
where Type = "Article"
SORT Progress asc
```
