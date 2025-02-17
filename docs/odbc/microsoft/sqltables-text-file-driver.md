---
title: "SQLTables (Text File Driver)"
description: "SQLTables (Text File Driver)"
author: David-Engel
ms.author: v-davidengel
ms.date: "01/19/2017"
ms.service: sql
ms.subservice: connectivity
ms.topic: conceptual
helpviewer_keywords:
  - "text file driver [ODBC], SQLTables"
  - "SQLTables function [ODBC], Text File Driver"
---
# SQLTables (Text File Driver)
> [!NOTE]  
>  This topic provides Text File Driver-specific information. For general information about this function, see the appropriate topic under [ODBC API Reference](../../odbc/reference/syntax/odbc-api-reference.md).  
  
|Argument|Comments|  
|--------------|--------------|  
|*szTableOwner*|The only valid argument for *szTableOwner* is NULL because none of the drivers support owner names. With *szTableOwner* set to NULL, all tables are returned. NULL is returned in the TABLE_OWNER column.|  
|*szTableQualifier*|In the TABLE_QUALIFIER column, **SQLTables** will return the path to a directory.|  
|*SzTableType*|"TABLE" is the only table type supported.<br /><br /> When the Text driver is used, the list of files returned by **SQLTables** is determined by the file extensions in the **Extensions List** box in the **ODBC Text Setup** dialog box.|
