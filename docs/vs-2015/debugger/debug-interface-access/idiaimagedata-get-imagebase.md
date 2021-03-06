---
title: "IDiaImageData::get_imageBase | Microsoft Docs"
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
  - "IDiaImageData::get_imageBase method"
ms.assetid: 4ba3d9e4-b205-4ee6-a41d-6996972f1f85
caps.latest.revision: 11
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# IDiaImageData::get_imageBase
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDiaImageData::get_imageBase](https://docs.microsoft.com/visualstudio/debugger/debug-interface-access/idiaimagedata-get-imagebase).  
  
Retrieves the memory location where the image should be based.  
  
## Syntax  
  
```cpp#  
HRESULT get_imageBase (   
   ULONGLONG* pRetVal  
);  
```  
  
#### Parameters  
 `pRetVal`  
 [out] Returns the suggested image base value.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## Remarks  
 Due to image base conflicts, an image may be rebased automatically to an unused memory location when it is loaded. This method returns the base hint (suggested memory location) that was stored in the module at compile time.  
  
## See Also  
 [IDiaImageData](../../debugger/debug-interface-access/idiaimagedata.md)



