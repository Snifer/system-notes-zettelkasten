---
Title: <% tp.system.prompt("Title Course", "")%>
Author: 
Tag: 
Url: <% tp.system.prompt("URL Course", "")%>
Status: <%tp.system.suggester(["Not Started", "In Progress", " Completed"], ["To Read", "Reading", "Completed"])%>
Type: Course
banner: "<%tp.system.prompt("URL image Course", "")%>"
banner_icon: 📖
banner_y: 0.236
Created: <%tp.date.now("MM-DD-YYYY", 7)%>
Total: 5
Incomplete: 5
Completed: 0
---


#  <%tp.system.prompt("Name Course", "")%>


> [!NOTE] ATENTION
> It's necessary to change the variable "a" with the Project start date and the variable "b" with the end date, in order to have a reference of the progress and time remaining.


> [!NOTE] ATENCION
> Es necesario cambiar la variable "a" por la fecha de inicio del proyecto y la variable "b" por la fecha de finalización, para tener una referencia del progreso y del tiempo restante.

%% PLEASE REMOVE THE CALLOUTS %%

```dataviewjs
var a = moment("2022-06-01"); 
var b = moment("2022-07-22");


var n = moment()
var t = moment().startOf('day');

let q =  b.diff(a, 'days');
let p =  b.diff(t, 'days');
let r =  t.diff(a, 'days');

let h = n.diff(a, 'hours');
let i = b.diff(a, 'hours');

let html = `<progress style="height:20px;width:100px" value="`+h+`" max="`+i+`"></progress>`

if (r>0 && r<q) {
	html += `\n#### `+p+` days left of `+q+` days\n`
	html += (h/i*100).toFixed(2)+`% complete`
} else if (r==0) {
	html += `\nstars today`
} else if (r==q) {
	html += `\nends today`
} else if (r>q) {
	html += `\nended `+-p+` days ago`
}else {
	html += `\n#### `+-r+` days to go`
}

dv.paragraph(html)
```

---


```button
name New Extract
type command
action QuickAdd: Summary
```

# Summary 



```dataview
TABLE 

Reference,
Type

FROM ([[<%tp.file.title%>]])
```




# Modules

## 1) CAPITULO 1

- [x] primeros pasos
- [ ] Segundos pasos


## 2) CAPITULO 2

- [ ] tareas
- [ ] revisiones
- [ ] tareas

