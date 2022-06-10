---
cssclass: dashboard, cards, center
banner: "https://scontent.fcbb1-1.fna.fbcdn.net/v/t31.18172-8/16715938_621432461394329_9173906849803471409_o.jpg?_nc_cat=111&ccb=1-7&_nc_sid=9267fe&_nc_ohc=HRdj0QE2-LkAX9y2jq_&_nc_ht=scontent.fcbb1-1.fna&oh=00_AT8VZSA0TV2zx0sEXknOXukXZO6jt6YCbn4MF1mxtDlVxw&oe=62BA5E4F"
banner_icon: 📖
banner_y: 0.236
---

- <mark style="background: #BBFABBA6;">[[Summary|🔍Extracts]]</mark> 
- [[000 Books|📚 Books]]
- [[000 Articles|📖 Articles]]
- [[000 Courses|📚 Courses]]
- [[000 Videos|📹 Videos]] 



```button
name New Register
type command
action QuickAdd: Library
```


# Library

```dataview
TABLE without id 
  ("![banner|50](" + banner + ")") as Cover,

  file.link AS "Title",
  Author AS "Author",
  Category AS "Category",
  Type, 
  Status,
  Rating AS Rating

 
FROM "Library"
where Type = "Book" or "Document" or "Video" and  !contains(file.name, "000")  and !contains(Type, "Quote") and !contains(Type, "Image") and !contains(Type, "Annotation") and !contains(Type, "Extract") and !contains(file.name, "Library") and !contains(file.name, "Summary") 
SORT Status asc
```

---

### Uso

Al momento de crear un nuevo registro debes de ser en miniscula el nombre de la nota.


### Agradecimientos




Gracias por descargar este Vault visitanos en <mark style="background: #ADCCFFA6;">[Snifer@L4b's](www.sniferl4bs.com)</mark> y siguenos en el Canal de <mark style="background: #ADCCFFA6;">[Youtube](https://youtube.com/c/sniferl4bs)</mark>, si tienes alguna sugerencia para mejorar el Vault escribenos  en sniferl4bs(arroba)gmail(punto)com.

Gracias a todos los que aportaron con su talento para que pueda unificar y tener este vault.

#### Temas y configuraciones de Obsidian

-  <mark style="background: #BBFABBA6;"> [Dashboard++](https://forum.obsidian.md/t/dashboard-a-simple-organization-and-navigation-method-for-obsidian-vaults/33197) </mark>
- <mark style="background: #ADCCFFA6;"> [Cards](https://github.com/kepano/obsidian-minimal ) </mark> 
-  <mark style="background: #ADCCFFA6;">[Project Tracking](https://forum.obsidian.md/t/project-tracking-templater-metaedit-and-dataview/19103)</mark> 
-  <mark style="background: #FFF3A3A6;">[Custom CSS Table](https://forum.obsidian.md/t/custom-css-for-tables-5-new-styles-ready-to-use-in-your-notes/17084)</mark> 
- <mark style="background: #BBFABBA6;"> [ Lectures Notes Progress Bar](https://forum.obsidian.md/t/university-setup-with-lecture-notes-progress-bar-and-more-using-templater-dataview-and-buttons/32094/4)</mark>

#### Sistema de Notas 

Los siguientes canales, con sus respectivos videos que se mencionan, fueron el motivo de llevar este flujo creado por Rubén Loan para Notion y migrado específicamente para Obsidian por mi persona, además de hacer algunos cambios adicionales visuales al mismo.

- [Ruben Loan ](https://www.youtube.com/watch?v=2rV13AhSHgs)
- [Ali Abbdad](https://www.youtube.com/watch?v=AjoxkxM_I5g)


Licencia   [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode)  ©2022


