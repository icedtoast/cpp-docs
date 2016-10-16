---
title: "RoInitializeWrapper Class"
ms.custom: na
ms.date: "10/14/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-cpp"
ms.tgt_pltfrm: na
ms.topic: "reference"
f1_keywords: 
  - "corewrappers/Microsoft::WRL::Wrappers::RoInitializeWrapper"
dev_langs: 
  - "C++"
ms.assetid: 4055fbe0-63a7-4c06-b5a0-414fda5640e5
caps.latest.revision: 2
ms.author: "mblome"
manager: "ghogen"
translation.priority.ht: 
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "ru-ru"
  - "zh-cn"
  - "zh-tw"
translation.priority.mt: 
  - "cs-cz"
  - "pl-pl"
  - "pt-br"
  - "tr-tr"
---
# RoInitializeWrapper Class
Initializes the [!INCLUDE[wrt](../atl/includes/wrt_md.md)].  
  
## Syntax  
  
```  
class RoInitializeWrapper  
```  
  
## Remarks  
 RoInitializeWrapper is a convenience that initializes the [!INCLUDE[wrt](../atl/includes/wrt_md.md)] and returns an HRESULT that indicates whether the operation was successful.  
  
## Members  
  
### Public Constructors  
  
|Name|Description|  
|----------|-----------------|  
|[RoInitializeWrapper::RoInitializeWrapper Constructor](../windows/roinitializewrapper--roinitializewrapper-constructor.md)|Initializes a new instance of the RoInitializeWrapper class.|  
|[RoInitializeWrapper::~RoInitializeWrapper Destructor](../windows/roinitializewrapper--~roinitializewrapper-destructor.md)|Destroys the current instance of the RoInitializeWrapper class.|  
  
### Public Operators  
  
|Name|Description|  
|----------|-----------------|  
|[RoInitializeWrapper::HRESULT() Operator](../windows/roinitializewrapper--hresult---operator.md)|Retrieves the HRESULT produced by the RoInitializeWrapper constructor.|  
  
## Inheritance Hierarchy  
 `RoInitializeWrapper`  
  
## Requirements  
 **Header:** corewrappers.h  
  
 **Namespace:** Microsoft::WRL::Wrappers  
  
## See Also  
 [Microsoft::WRL::Wrappers Namespace](../windows/microsoft--wrl--wrappers-namespace.md)