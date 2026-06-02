---
title: "How to convert a flat parent-child list from database into a nested tree structure for JSON response in Spring Boot?"
url: "https://stackoverflow.com/questions/79947460/how-to-convert-a-flat-parent-child-list-from-database-into-a-nested-tree-structu"
date: "2026-05-27"
author: "Oscar Sandoval"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
When calling my API endpoint, the default repository output returns a flat list array like this [ { "id": "root_postgres", "name": "Main Root", "type": "FOLDER", "parentId": null }, { "id": "exams_folder", "name": "Exams", "type": "FOLDER", "parentId": "root_postgres" } ] But i want a deeply neste JSON tree structure like this { "id": "root_postgres", "value": "Main Root", "children": [ { "id": "exams_folder", "value": "Exams", "children": [] } ] } What is the cleanest algorithmic approach or architectural pattern in a Spring @Service to index these database rows dynamically, preferably in O(1
