---
title: "Changing entity type from List<T> to Set<T> in manytomany causes spring app to throw concurrentModificationException"
url: "https://stackoverflow.com/questions/79981173/changing-entity-type-from-listt-to-sett-in-manytomany-causes-spring-app-to-t"
date: "2026-07-16"
author: "Tapialj"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I am attempting to correct a mistake in how a ManyToMany relationship is set up and change the Lists over to Sets as I've read. But when I change each side of the relationship to a set, it breaks the jpa repository it seems. Any query to to the repository will throw the concurrentModificationException.
