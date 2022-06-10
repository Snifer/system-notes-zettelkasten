---
cssclass: academia, academia-rounded, cards, dashboard
banner: "https://i.pinimg.com/originals/82/05/37/820537a0481569f61858a7fa00f85ec8.jpg"
banner_icon: 📚
banner_y: 0.132
---
# Courses
- [[000 Library|🗄️ Library]]
- [[000 Books|📚 Books]]
- [[000 Articles|📖 Articles]]
- [[000 Courses|📚 Courses]]
- [[000 Videos|📹 Videos]]

```dataview
TABLE without id 
  ("![cover|90](" + banner + ")") as Cover,
  file.link AS "Title",
  Author AS "Author",
  Category AS "Category",
  Type, 
  Status,
  Rating AS Rating

 
FROM "Library/Course"
where Type = "Course"
SORT Progress asc
```


