# Mains
```dataview
table title, tags, subject
where type = "Note Hub"
sort file.mtime desc
```

# Published
```dataview
table title, file.folder, file.mday
where publish = true
sort subject asc, file.mtime desc
```