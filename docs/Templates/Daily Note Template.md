---
tags:
  - dailies
---
## <% moment(tp.file.title, "YYYY-MM-DD").format("dddd Do MMMM YYYY") %>

<< [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD').subtract(1, 'd').format('YYYY-MM-DD') %>|Yesterday]] | [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD').add(1, 'd').format('YYYY-MM-DD') %>|Tomorrow]] >>

````col
height=50
===
```col-md
> [!success]+ Tasks Done Today  
> ```tasks  
> done %3C% tp.date.now("YYYY-MM-DD") %>  
> hide due date  
> hide backlink
```

```col-md

> [!todo]+ Today's Tasks  
> ```tasks  
> not done  
> due %3C% tp.date.now("YYYY-MM-DD") %>  
> sort by priority  
> hide due date  
> hide backlink  
> limit 5  
> ```
```
````

````col
height=50
===
```col-md
> [!warning]+ OverDue  
> ```tasks  
> not done  
> sort by due date  
> due before %3C% tp.date.now("YYYY-MM-DD") %>  
> hide due date  
> hide backlink  
> limit 5  
> ```
```

```col-md

> [!Warning]+ Unscheduled Tasks  
> ```tasks  
> not done  
> no due date
> ```
```
````

````col
height=50
===
```col-md
> [!tip]+ Habit Tracker  
> Toofs:: 0  
> SSRI:: 0  
> ADHD:: 0  
> Food:: 0  
> Writing:: 0
> BP:: 0
> Scales:: 0
> Bed:: 0
```

```col-md
> [!tip] Health
> sysdias:: 0/0 / 09:00AM
> weight:: 85kg / 09:00AM
```
````







## New Task
