---
title: "Options (SQL Server Object Explorer - Commands)"
description: "Options (SQL Server Object Explorer - Commands)"
author: "markingmyname"
ms.author: "maghan"
ms.date: 04/11/2023
ms.service: sql
ms.subservice: ssms
ms.topic: conceptual
f1_keywords:
  - "VS.ToolsOptionsPages.SQL_Server_Object_Explorer.Commands"
---

# Options (SQL Server Object Explorer - Commands)

[!INCLUDE[SQL Server Azure SQL Database Synapse Analytics PDW](../../includes/applies-to-version/sql-asdb-asdbmi-asa-pdw.md)]

When you right-click a table or view in Object Explorer, the following two options for displaying rows in the table are presented:

- **Select Top 1000 Rows**

    Creates a script in the Query Editor that selects the top 1000 rows.

- **Edit Top 200 Rows**

    Opens the table in the Visual Database Tools with 200 rows populated.

Use the **General Scripting Options** dialog box to change the number of rows that will be opened.

## General Scripting Options

**Value for Select Top \<n\> Audit record command**  
Specifies the number of audit rows to return. The default is 1000 rows

**Value for Edit Top \<n\> Rows command**  
Specifies the number of rows to return when you are editing rows in a table. The default is 200 rows.

**Value for Select Top \<n\> Rows command**  
Specifies the number of rows to be returned that is specified in the Query Editor script that is created. The default is 1000 rows.

## Next setps

- [SQL Server Audit (Database Engine)](../../relational-databases/security/auditing/sql-server-audit-database-engine.md)
