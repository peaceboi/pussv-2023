---
aliases: 
tags: [projects, graphic-design]
---

```dataview
list 
where contains(projects, "graphic-design")
```



>[!info]
> The following code block allows you to "freeze" the Dataview query result above into HTML.
> If you use Obsidian Publish, this will allow you to publish the resource list as it is above.
> I recommend running this, **after** you finish a project and are ready to commit it to _PARA/Archive.
> To use: open command pallette, remove the spaces between < % and *, run "Templater: Replace all templates in Active File", and remove the triple backticks.

```
< % *
const dv = this.app.plugins.plugins["dataview"].api ;
const arr = await dv.queryMarkdown('LIST where contains(projects, "graphic-design")')
tR += arr.value
% >
```

