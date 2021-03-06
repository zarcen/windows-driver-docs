---
title: ISNMP Automation Interface
author: windows-driver-content
description: ISNMP Automation Interface
MS-HAID:
- 'webfnc\_4ff82461-8ece-4336-8f86-9461ad4ec8d7.xml'
- 'print.isnmp\_automation\_interface'
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 63f2f14d-ea9d-437c-9853-06889219627d
ms.localizationpriority: medium
---

# ISNMP Automation Interface


## <span id="ddk_isnmp_automation_interface_gg"></span><span id="DDK_ISNMP_AUTOMATION_INTERFACE_GG"></span>


The Automation interface for the **ISNMP** object is essentially an OLE automation wrapper for the functions in the Simple Network Management Protocol (SNMP) Management API. The **ISNMP** interface enables an ASP Web page to set and retrieve values associated with SNMP object identifiers (OIDs). For more information about the SNMP Management API, see the Windows SDK documentation.

The **ISNMP** interface works only with printers that use Microsoft's standard TCIP/IP [*port monitor*](https://msdn.microsoft.com/library/windows/hardware/ff556325#wdkgloss-port-monitor). **ISNMP** is supported in Microsoft Windows 2000 and later versions of Windows. (However, the [**ISNMP::GetAsByte**](isnmp-getasbyte.md) property is supported only in Windows XP and later versions of Windows.)

The programmatic identifier for the **ISNMP** object is OlePrn.OleSNMP.

For more information about how to access printers from ASP Web pages, see [Internet Printing](https://msdn.microsoft.com/library/windows/hardware/ff551735).

The methods in the **ISNMP** interface are described in the following section:

[ISNMP Methods](isnmp-methods.md)

 

 




