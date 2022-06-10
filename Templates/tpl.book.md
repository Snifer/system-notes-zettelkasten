---
cssclass: academia, academia-rounded, center
Title: <% tp.system.prompt("Title Book", "")%>
Author: 
Status: <%tp.system.suggester([" To Read", "Reading", " Completed"], ["To Read", "Reading", "Completed"])%>
Type: <%tp.system.suggester(["📖 Book", "📃 Document"], ["Book", "Document"])%>
Rating: 
Category: 
Pages: <%tp.system.prompt("Total Pages", "")%>
banner: "<%tp.system.prompt("URL Cover", "")%>"
banner_icon: 📖
banner_y: 0.236
Created: <%tp.date.now("YYYY-MM-DD", 7)%>
Finish_Read:
---

# <%tp.system.prompt("Title Header", "")%>


- Total Pages Read  
	- **PagesRead**:: <%tp.system.prompt("Read Pages", "")%>
-  Avance Actual
 ```dataview
TABLE without id 

  ("![progress + " + (round((PagesRead/Pages)*100)) + " %](https://progress-bar.dev/" +(round((PagesRead/Pages)*100)) + "/)") AS ""

 
FROM "Library/Books/<% tp.file.title %>"
```

%%Paginas leidas agregar un boton para modificar la metadata Obsidian %% 

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









