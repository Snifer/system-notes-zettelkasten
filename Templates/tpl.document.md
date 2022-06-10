---
Title: <% tp.system.prompt("Title Index", "")%>
Tag: 
Type: 📝 Document
banner: "https://t3.ftcdn.net/jpg/01/05/85/14/360_F_105851441_gDJSXUgfH54DwX5rfH6Qiq4sHIZ9ogYL.jpg"
banner_icon: 📖
banner_y: 0.236
Created: <%tp.date.now("MM-DD-YYYY", 7)%>
Reference: 
---


```button
name New Extract
type command
action QuickAdd: Extracts
```


## Summary 


```dataview
TABLE 

Reference,
Type

FROM ([[<% tp.file.title %>]])
```


