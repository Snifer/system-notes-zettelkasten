---
Title: <% tp.system.prompt("Title Article", "")%>
Author: 
Url: <% tp.system.prompt("URL Article", "")%>
Status: <%tp.system.suggester([" To Read", "Reading", " Completed"], ["To Read", "Reading", "Completed"])%>
Type: Article
banner: "<%tp.system.prompt("URL Cover", "")%>"
banner_icon: 📖
banner_y: 0.236
Created: <%tp.date.now("YYYY-MM-DD", 7)%>
Reference:
Tag:

---



```button
name New Extract
type command
action QuickAdd: Summary
```


## Summary 


```dataview
TABLE 
Reference, 
Type

FROM ([[<%tp.file.title%>]])
```

