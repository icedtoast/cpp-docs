---
title: "time_put_byname Class"
ms.custom: na
ms.date: "10/14/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-cpp"
ms.tgt_pltfrm: na
ms.topic: "article"
f1_keywords: 
  - "time_put_byname"
  - "xloctime/std::time_put_byname"
  - "std.time_put_byname"
  - "std::time_put_byname"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "time_put_byname class"
ms.assetid: e08c2348-64d2-4ace-98b1-1496e14c7b1a
caps.latest.revision: 24
ms.author: "corob"
manager: "ghogen"
translation.priority.mt: 
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
# time_put_byname Class
The derived template class describes an object that can serve as a locale facet of type `time_put`\< CharType, OutputIterator >.  
  
## Syntax  
  
```
template<class CharType, class OutIt = ostreambuf_iterator<CharType, char_traits<CharType>>>
class time_put_byname : public time_put<CharType, OutputIterator>
{
public:
    explicit time_put_byname(
    const char* _Locname,
    size_t _Refs = 0);

    explicit time_put_byname(
    const string& _Locname,
    size_t _Refs = 0);

protected:
    virtual ~time_put_byname();

};
```  
  
#### Parameters  
 `_Locname`  
 A locale name.  
  
 `_Refs`  
 An initial reference count.  
  
## Remarks  
 Its behavior is determined by the [named](../stdcpplib/locale-class.md#locale__name) locale `_Locname`. Each constructor initializes its base object with [time_put](../stdcpplib/time_put-class.md#time_put__time_put)\<CharType, OutputIterator>( `_Refs`).  
  
## Requirements  
 **Header:** \<locale>  
  
 **Namespace:** std  
  
## See Also  
 [Thread Safety in the C++ Standard Library](../stdcpplib/thread-safety-in-the-c---standard-library.md)
