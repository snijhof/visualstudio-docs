---
title: "CA1703: Resource strings should be spelled correctly | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-code-analysis"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "ResourceStringsShouldBeSpelledCorrectly"
  - "CA1703"
helpviewer_keywords: 
  - "CA1703"
  - "ResourceStringsShouldBeSpelledCorrectly"
ms.assetid: 693f4970-f512-40cb-ae3b-a0f3a5c6d6f1
caps.latest.revision: 16
author: "gewarren"
ms.author: "gewarren"
manager: ghogen
ms.workload: 
  - "multiple"
---
# CA1703: Resource strings should be spelled correctly
|||  
|-|-|  
|TypeName|ResourceStringsShouldBeSpelledCorrectly|  
|CheckId|CA1703|  
|Category|Microsoft.Naming|  
|Breaking Change|Non-breaking|  
  
## Cause  
 A resource string contains one or more words that are not recognized by the Microsoft spelling checker library.  
  
## Rule Description  
 This rule parses the resource string into words (tokenizing compound words) and checks the spelling of each word/token. For information about the parsing algorithm, see [CA1704: Identifiers should be spelled correctly](../code-quality/ca1704-identifiers-should-be-spelled-correctly.md).  
  
 By default, the English (en) version of the spelling checker is used.  
  
## How to Fix Violations  
 To fix a violation of this rule, use complete words that are correctly spelled or add the words to a custom dictionary. For information about how to use custom dictionaries, see [CA1704: Identifiers should be spelled correctly](../code-quality/ca1704-identifiers-should-be-spelled-correctly.md).  
  
## When to Suppress Warnings  
 Do not suppress a warning from this rule. Correctly spelled words reduce the time that is required to learn new software libraries.  
  
## Related Rules  
 [CA1701: Resource string compound words should be cased correctly](../code-quality/ca1701-resource-string-compound-words-should-be-cased-correctly.md)  
  
 [CA1704: Identifiers should be spelled correctly](../code-quality/ca1704-identifiers-should-be-spelled-correctly.md)  
  
 [CA2204: Literals should be spelled correctly](../code-quality/ca2204-literals-should-be-spelled-correctly.md)