![](05%20Archivo/Plantillas/pachakamani.jpg)
## Contenido del PKM

>[!todo]- Estadísticas:
>- Total Notas: `$=dv.pages().length`
>- Etiquetas MOC: `$=dv.pages('#moc').length`
>- Proyectos: `$=dv.pages('"00 LIBRETA/PROYECTOS"').length`
>- Total notas de IDEA: `$=dv.pages('"01 IDEAS"').length`
>- Referencias: `$=dv.pages('"02 REFERENCIAS"').length`

>[!check]- Notas de Idea
>``` dataview
>TABLE
>file.cday as "Creada"
>FROM "01 IDEAS"  
>SORT file.ctime DESC
>```

>[!note]- Referencias 
>```dataview
>TABLE
>file.cday as "Creada"
>FROM "02 REFERENCIAS"  
>SORT file.mtime DESC
>```

>[!todo]- Mapas de Contenido
>``` dataview
>TABLE
>file.cday as "Creada"
>FROM "03 MOC"  
>SORT file.ctime DESC
>```

>[!check]- Proyectos 
>``` dataview
>TABLE
>file.cday as "Creada"
>FROM "00 LIBRETA/PROYECTOS"  
>SORT file.ctime DESC
>```

[[0 Mapa de Proyectos. Kanban]]