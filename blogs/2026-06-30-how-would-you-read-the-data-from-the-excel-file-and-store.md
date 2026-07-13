---
title: "How would you read the data from the Excel file and store it into a database using Java?"
url: "https://stackoverflow.com/questions/79971563/how-would-you-read-the-data-from-the-excel-file-and-store-it-into-a-database-usi"
date: "2026-06-30"
author: "Mahadev Jangam"
feed_url: "https://stackoverflow.com/feeds/tag?tagnames=spring-boot&sort=newest"
---
You have an Excel (.xls/.xlsx) file containing 1000 employee records. How would you read the data from the Excel file and store it into a database using Java? org.apache.poi poi-ooxml 5.4.1 FileInputStream fis = new FileInputStream("employees.xlsx"); Workbook workbook = new XSSFWorkbook(fis); Sheet sheet = workbook.getSheetAt(0); for(Row row : sheet) { int empId = (int) row.getCell(0).getNumericCellValue(); String name = row.getCell(1).getStringCellValue(); String email = row.getCell(2).getStringCellValue(); double salary = row.getCell(3).getNumericCellValue(); }
