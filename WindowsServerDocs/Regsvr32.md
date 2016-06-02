---
title: Regsvr32
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 3345e964-7d3e-42b8-abeb-42ed6edfe2b2
author: jaimeo
---
# Regsvr32
Registers .dll files as command components in the registry.  
  
For examples of how to use this command, see [Examples](#BKMK_examples).  
  
## Syntax  
  
```  
regsvr32 [/u] [/s] [/n] [/i[:cmdline]] <DllName>  
```  
  
## Parameters  
  
|Parameter|Description|  
|-------------|---------------|  
|\/u|Unregisters server.|  
|\/s|Runs **Regsvr32** without displaying messages.|  
|\/n|Runs **Regsvr32** without calling **DllRegisterServer**. \(Requires the **\/i** parameter.\)|  
|\/i:<cmdline>|Passes an optional command\-line string \(*cmdline*\) to **DllInstall**. If you use this parameter in conjunction with the **\/u** parameter, it calls **DllUninstall**.|  
|<DllName>|The name of the .dll file that will be registered.|  
|\/?|Displays help at the command prompt.|  
  
## <a name="BKMK_examples"></a>Examples  
To register the .dll for the Active Directory Schema, type:  
  
```  
regsvr32 schmmgmt.dll  
```  
  
#### Additional references  
[Command-Line Syntax Key](Command-Line-Syntax-Key.md)  
  
