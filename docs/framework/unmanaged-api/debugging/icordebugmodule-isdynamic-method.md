---
title: "ICorDebugModule::IsDynamic Method | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "reference"
apiname: 
  - "ICorDebugModule.IsDynamic"
apilocation: 
  - "mscordbi.dll"
apitype: "COM"
f1_keywords: 
  - "ICorDebugModule::IsDynamic"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "IsDynamic method [.NET Framework debugging]"
  - "ICorDebugModule::IsDynamic method [.NET Framework debugging]"
ms.assetid: 5eefe716-5025-4a4c-970c-c823cdc7bb87
caps.latest.revision: 10
author: "rpetrusha"
ms.author: "ronpet"
manager: "wpickett"
---
# ICorDebugModule::IsDynamic Method
Gets a value that indicates whether this module is dynamic.  
  
## Syntax  
  
```  
HRESULT IsDynamic(  
    [out] BOOL *pDynamic  
);  
```  
  
#### Parameters  
 `pDynamic`  
 [out] `true` if this module is dynamic; otherwise, `false`.  
  
## Remarks  
 A dynamic module can add new classes and delete existing classes even after the module has been loaded. The [ICorDebugManagedCallback::LoadClass](../../../../docs/framework/unmanaged-api/debugging/icordebugmanagedcallback-loadclass-method.md) and [ICorDebugManagedCallback::UnloadClass](../../../../docs/framework/unmanaged-api/debugging/icordebugmanagedcallback-unloadclass-method.md) callbacks inform the debugger when a class has been added or deleted.  
  
## Requirements  
 **Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).  
  
 **Header:** CorDebug.idl, CorDebug.h  
  
 **Library:** CorGuids.lib  
  
 **.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]