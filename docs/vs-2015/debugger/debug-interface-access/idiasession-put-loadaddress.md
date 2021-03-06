---
title: "IDiaSession::put_loadAddress | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "IDiaSession::put_loadAddress method"
ms.assetid: b157b245-1ea0-4b80-8962-d8b278dbc742
caps.latest.revision: 14
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# IDiaSession::put_loadAddress
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDiaSession::put_loadAddress](https://docs.microsoft.com/visualstudio/debugger/debug-interface-access/idiasession-put-loadaddress).  
  
Sets the load address for the executable file that corresponds to the symbols in this symbol store.  
  
## Syntax  
  
```cpp#  
HRESULT put_loadAddress (   
   ULONGLONG NewVal  
);  
```  
  
#### Parameters  
 `NewVal`  
 [in] Load address for the executable file.  
  
## Remarks  
 Symbol virtual address (VA) properties are computed using the value of this method. Virtual addresses are not calculated unless this property is set to non-zero.  
  
> [!NOTE]
>  You must call this method when you get the [IDiaSession](../../debugger/debug-interface-access/idiasession.md) object and before you start using the object if you need to use any virtual properties on symbols.  
  
## See Also  
 [IDiaSession](../../debugger/debug-interface-access/idiasession.md)



