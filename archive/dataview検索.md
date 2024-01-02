skill
フィルタリングはcontainsで行う

```dataview
TABLE rows.file.link,rows.file.tags
where file.inlinks
where type = "skill"
where contains(file.tags,"体力")
group by file.inlinks
```

```dataviewjs
console.log(await dv.queryMarkdown(`TABLE rows.file.link,rows.file.tags
where file.inlinks
where type = "skill"
where contains(file.tags,"体力")
group by file.inlinks`))
```


