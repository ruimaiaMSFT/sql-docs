---
title: "sp_syspolicy_purge_health_state (Transact-SQL)"
description: "sp_syspolicy_purge_health_state (Transact-SQL)"
author: VanMSFT
ms.author: vanto
ms.date: "03/14/2017"
ms.service: sql
ms.subservice: system-objects
ms.topic: "reference"
f1_keywords:
  - "sp_syspolicy_purge_health_state_TSQL"
  - "sp_syspolicy_purge_health_state"
helpviewer_keywords:
  - "sp_syspolicy_purge_health_state"
dev_langs:
  - "TSQL"
---
# sp_syspolicy_purge_health_state (Transact-SQL)
[!INCLUDE [SQL Server](../../includes/applies-to-version/sqlserver.md)]

  Deletes the policy health states in Policy-Based Management. Policy health states are visual indicators (a scroll symbol with a red "X") within Object Explorer that enable you to determine which nodes have failed a policy evaluation.  
  
 :::image type="icon" source="../../includes/media/topic-link-icon.svg" border="false"::: [Transact-SQL syntax conventions](../../t-sql/language-elements/transact-sql-syntax-conventions-transact-sql.md)  
  
## Syntax  
  
```  
  
sp_syspolicy_purge_health_state [ @target_tree_root_with_id = ] 'target_tree_root_with_id'  
```  
  
## Arguments  
`[ @target_tree_root_with_id = ] 'target_tree_root_with_id'`
 Represents the node in Object Explorer where you want to clear the health state. *target_tree_root_with_id* is **nvarchar(400)**, with a default of NULL.  
  
 You can specify values from the target_query_expression_with_id column of the msdb.dbo.syspolicy_system_health_state system view.  
  
## Return Code Values  
 **0** (success) or **1** (failure)  
  
## Remarks  
 You must run sp_syspolicy_purge_health_state in the context of the msdb system database.  
  
 If you run this stored procedure without any parameters, the system health state is deleted for all nodes in Object Explorer.  
  
## Permissions  
 Requires membership in the PolicyAdministratorRole fixed database role.  
  
> [!IMPORTANT]  
>  Possible elevation of credentials: Users in the PolicyAdministratorRole role can create server triggers and schedule policy executions that can affect the operation of the instance of the [!INCLUDE[ssDE](../../includes/ssde-md.md)]. For example, users in the PolicyAdministratorRole role can create a policy that can prevent most objects from being created in the [!INCLUDE[ssDE](../../includes/ssde-md.md)]. Because of this possible elevation of credentials, the PolicyAdministratorRole role should be granted only to users who are trusted with controlling the configuration of the [!INCLUDE[ssDE](../../includes/ssde-md.md)].  
  
## Examples  
 The following example deletes the health states for a specific node in Object Explorer.  
  
```  
EXEC msdb.dbo.sp_syspolicy_purge_health_state @target_tree_root_with_id = 'Server/Database[@ID=7]';  
  
GO  
```  
  
## See Also  
 [Policy-Based Management Stored Procedures &#40;Transact-SQL&#41;](../../relational-databases/system-stored-procedures/policy-based-management-stored-procedures-transact-sql.md)  
  
  
