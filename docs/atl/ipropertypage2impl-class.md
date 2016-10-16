---
title: "IPropertyPage2Impl Class"
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
  - "IPropertyPage2Impl"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "property pages"
  - "IPropertyPage2 ATL implementation"
  - "IPropertyPage2Impl class"
ms.assetid: e89fbe90-203a-47f0-a5de-23616697e1ce
caps.latest.revision: 15
ms.author: "mblome"
manager: "ghogen"
translation.priority.ht: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# IPropertyPage2Impl Class
This class implements **IUnknown** and inherits the default implementation of [IPropertyPageImpl](../atl/ipropertypageimpl-class.md).  
  
> [!IMPORTANT]
>  This class and its members cannot be used in applications that execute in the [!INCLUDE[wrt](../atl/includes/wrt_md.md)].  
  
## Syntax  
  
```
template<class T>  class IPropertyPage2Impl : public IPropertyPageImpl<T>
```  
  
#### Parameters  
 `T`  
 Your class, derived from `IPropertyPage2Impl`.  
  
## Members  
  
### Public Methods  
  
|Name|Description|  
|----------|-----------------|  
|[IPropertyPage2Impl::EditProperty](../Topic/IPropertyPage2Impl::EditProperty.md)|Specifies which property control will receive the focus when the property page is activated. The ATL implementation returns **E_NOTIMPL**.|  
  
## Remarks  
 The [IPropertyPage2](http://msdn.microsoft.com/library/windows/desktop/ms683996) interface extends [IPropertyPage](http://msdn.microsoft.com/library/windows/desktop/ms691246) by adding the `EditProperty` method. This method allows a client to select a specific property in a property page object.  
  
 Class `IPropertyPage2Impl` simply returns **E_NOTIMPL** for **IPropertyPage2::EditProperty**. However, it inherits the default implementation of [IPropertyPageImpl](../atl/ipropertypageimpl-class.md) and implements **IUnknown** by sending information to the dump device in debug builds.  
  
 When you create a property page, your class is typically derived from `IPropertyPageImpl`. To provide the extra support of **IPropertyPage2**, modify your class definition and override the `EditProperty` method.  
  
 **Related Articles** [ATL Tutorial](../atl/active-template-library--atl--tutorial.md), [Creating an ATL Project](../atl/creating-an-atl-project.md)  
  
## Inheritance Hierarchy  
 `IPropertyPage`  
  
 [IPropertyPageImpl](../atl/ipropertypageimpl-class.md)  
  
 `IPropertyPage2Impl`  
  
## Requirements  
 **Header:** atlctl.h  
  
##  <a name="ipropertypage2impl__editproperty"></a>  IPropertyPage2Impl::EditProperty  
 Specifies which property control will receive the focus when the property page is activated.  
  
```
HRESULT EditProperty(DISPID dispID);
```  
  
### Return Value  
 Returns **E_NOTIMPL**.  
  
### Remarks  
 See [IPropertyPage2::EditProperty](http://msdn.microsoft.com/library/windows/desktop/ms690353) in the [!INCLUDE[winSDK](../atl/includes/winsdk_md.md)].  
  
## See Also  
 [IPerPropertyBrowsingImpl Class](../atl/iperpropertybrowsingimpl-class.md)   
 [ISpecifyPropertyPagesImpl Class](../atl/ispecifypropertypagesimpl-class.md)   
 [Class Overview](../atl/atl-class-overview.md)
