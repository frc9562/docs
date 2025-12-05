---
title: <% tp.file.title %>
aliases:
created: <% tp.file.creation_date("YYYY/MM/DD") %>
modified: <% tp.file.last_modified_date("YYYY/MM/DD") %>
tags:
  - quick-note
draft: true
todo: true
---
<% tp.file.cursor(1) %>
##  <% tp.file.title %>
<% tp.file.cursor(2) %>
## References
<% tp.file.cursor(3) %>