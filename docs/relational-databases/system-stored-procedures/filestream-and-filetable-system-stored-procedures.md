---
title: "Filestream and FileTable System Stored Procedures (Transact-SQL)"
description: "Filestream and FileTable System Stored Procedures (Transact-SQL)"
author: "MashaMSFT"
ms.author: "mathoma"
ms.date: "03/06/2017"
ms.service: sql
ms.subservice: system-objects
ms.topic: "reference"
helpviewer_keywords:
  - "FileTables [SQL Server], catalog views"
dev_langs:
  - "TSQL"
---
# Filestream and FileTable system stored procedures (Transact-SQL)
[!INCLUDE [SQL Server](../../includes/applies-to-version/sqlserver.md)]

  This section describes the system stored procedures to the FileTable and Filestream feature.  

## Filestream and Filetable system stored procedures
  [sp_filestream_force_garbage_collection (Transact-SQL)](filestream-and-filetable-sp-filestream-force-garbage-collection.md)

   Forces the FILESTREAM garbage collector to run, deleting any unneeded FILESTREAM files.

  [sp_kill_filestream_non_transacted_handles (Transact-SQL)](filestream-and-filetable-sp-kill-filestream-non-transacted-handles.md)

  Closes non-transactional file handles to FileTable data.


## See also
[Filestream](../../relational-databases/blob/filestream-sql-server.md)
<br>[Filetables](../../relational-databases/blob/filetables-sql-server.md)
<br>[Filestream and FileTable Dynamic Management Views (Transact-SQL)](../system-dynamic-management-views/filestream-and-filetable-dynamic-management-views-transact-sql.md)
<br>[Filestream and FileTable Catalog Views (Transact-SQL)](../system-catalog-views/filestream-and-filetable-catalog-views-transact-sql.md)
  
  
