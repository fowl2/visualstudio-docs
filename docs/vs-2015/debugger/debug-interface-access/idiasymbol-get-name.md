---
title: "IDiaSymbol::get_name | Microsoft Docs"
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
  - "IDiaSymbol::get_name method"
ms.assetid: 050ec02f-b7b3-48fc-8e35-58bdf7d938b0
caps.latest.revision: 11
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# IDiaSymbol::get_name
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDiaSymbol::get_name](https://docs.microsoft.com/visualstudio/debugger/debug-interface-access/idiasymbol-get-name).  
  
Retrieves the name of the symbol.  
  
## Syntax  
  
```cpp#  
HRESULT get_name (   
   BSTR* pRetVal  
);  
```  
  
#### Parameters  
 `pRetVal`  
 [out] Returns the name of the symbol.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns `S_FALSE` or an error code.  
  
> [!NOTE]
>  A return value of `S_FALSE` means the property is not available for the symbol.  
  
## Example  
  
```cpp#  
IDiaSymbol* pType;  
BSTR        name;  
pType->get_name( &name );  
```  
  
## See Also  
 [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)



