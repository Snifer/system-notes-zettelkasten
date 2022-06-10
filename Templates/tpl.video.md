---
cssclass: academia, academia-rounded, center
Title: <% tp.system.prompt("Title Video", "")%>
Author: 
Status:  <%tp.system.suggester(["Not Started", "In Progress", "Completed"], ["Not Started", "In Progress", "Completed"])%>
Type: 📽️ Video
Tag:
Created: <%tp.date.now("MM-DD-YYYY", 7)%>
banner: "<%tp.system.prompt("Miniature Video URL", "")%>"
banner_icon: 📽️
banner_y: 0.236
Created: <%tp.date.now("YYYY-MM-DD", 7)%>
---

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/<%tp.system.prompt("YouTube code E.g (2rV13ahS2gs) ", "")%>" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></center>

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

FROM ([[<% tp.file.title %>]])
```


