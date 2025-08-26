---
tags:
  - Mains
---
# Projects
These are the ‘Now’ things. Your current assignments, the novel you’re writing, or the vacation you’re planning. Like a to-do list that’s alive and breathing.  

[[CET Things]]
[[SUMMER CLEANING na naudlot putanginang bahay to]]

# Areas
Ongoing responsibilities or interests fall here. Your health, relationships, or the blog you regularly update. It’s like your life’s dashboard.

```dataview
table title, tags, subject
where type = "Note Hub"
sort file.mtime desc
```

**NORMAL SCHOOL NOTES**
# Resources
Collection of stuff that doesn’t need immediate action but is valuable. Your favorite recipes, e-books, or industry reports. Imagine a treasure chest of information you can dive into whenever. 

[[Movie Watchlist]]
[[Games]]
[[Books]]
[[Fanfics]]

```dataview
list title 
where contains(tags,"Mains")
sort file.mtime desc
```

**WORKOUT STUFF**

# Archives
Old projects, completed tasks, or past interests. Remember that college project from five years ago? It goes here. Think of it as a digital attic.

#DailyNotes and **TEMPLATES** and **zzMisc notes** 

```dataview
list title
where contains(tags,"CloverFolders") OR contains(tags,"DailyNotes")
sort file.mday desc, file.folder asc, date desc
```
