---
cssclass:  academia-rounded, dashboard
banner: "https://foodtank.com/wp-content/uploads/2021/07/alfons-morales-YLSwjSy7stw-unsplash.jpg"
banner_icon: 📖
banner_y: 0.236
---

# Books
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
  ("![banner|90](" + banner + ")") as Cover,
  ("![progress + " + (round((PagesRead/Pages)*100)) + " %](https://progress-bar.dev/" +(round((PagesRead/Pages)*100)) + "/)") AS Progress,
 
  file.link AS "Title",
  Author AS "Author",
  Category AS "Category",
  Type, 
  Status,
  Rating AS Rating

 
FROM "Library"
where Type = "Book" or "Document"
SORT Status asc
```
