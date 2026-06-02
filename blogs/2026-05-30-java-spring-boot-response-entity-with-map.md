---
title: "Java Spring Boot response entity with map"
url: "https://stackoverflow.com/questions/79948839/java-spring-boot-response-entity-with-map"
date: "2026-05-30"
author: "mikelauskas"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
I have the following code that creates a ResponseEntity for the response of a Spring app. Is there any more efficient way of doing this method? @GetMapping("/api/payments/reservation/{idReservation}") public ResponseEntity > obtenerPagoReal(@PathVariable("idReservation") int idReservation) { Payment pay = dao_interface.findByIdReserva(idReservation); Map response = new HashMap<>(); if (pago!=null) { response.put("status", "success"); response.put("code", 200); response.put("message", "Payment done"); response.put("data", pay); return ResponseEntity.ok(response); } else { response.put("status",
