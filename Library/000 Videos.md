---
cssclass: academia, academia-rounded, cards, dashboard
banner: "https://www.cyborgservices.in/wp-content/uploads/2017/11/video-banner-1.png"
banner_icon: 📹
banner_y: 0.36
---

# Articles
- [[Library/Videos/000 Library|🗄️ Library]]
- [[000 Books|📚 Books]]
- [[000 Articles|📖 Articles]]
- [[000 Courses|📚 Courses]]
- [[000 Videos|📹 Videos]]



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

 
FROM "Library/Videos"
where Type = "Video"
SORT Status asc
```
