---
title: "How to rebuild a tree from PostgreSQL without duplicate nodes? [closed]"
url: "https://stackoverflow.com/questions/79948263/how-to-rebuild-a-tree-from-postgresql-without-duplicate-nodes"
date: "2026-05-29"
author: "MARIO JOSE BARRERA LINAREZ"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I'm developing a Spring Boot application that stores a tree structure in PostgreSQL. The table schema is: CREATE TABLE nodes ( id BIGINT PRIMARY KEY, value VARCHAR(150), parent_id BIGINT ); Example data: 1 | Management | NULL 2 | IT Department | 1 3 | Developer | 2 To rebuild the tree in memory, I'm using Java Collections: private final Map > tree = new HashMap<>(); public void loadTree(List nodes) { for (NodeEntity node : nodes) { if (node.getParentId() != null) { tree.putIfAbsent(node.getParentId(), new ArrayList<>()); tree.get(node.getParentId()).add(node.getId()); } } } The problem is that
