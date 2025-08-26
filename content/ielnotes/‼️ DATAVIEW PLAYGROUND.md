# Mains
```dataview
table title, subject, file.folder
where type = "Note Hub"
sort file.mtime desc
```

# Published
```dataview
table title, file.folder, file.mday
where publish = true
sort file.mday desc, subject desc, title desc
```