---
title: IPrinterScriptUsbJobContext PrintedPageCount method
author: windows-driver-content
description: Sets the number of pages that have been printed by the print device in the current job.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 3C1DAE22-F1DF-48AE-A6F6-CCB8A97EB424
keywords: ["PrintedPageCount method Print Devices", "PrintedPageCount method Print Devices , IPrinterScriptUsbJobContext interface", "IPrinterScriptUsbJobContext interface Print Devices , PrintedPageCount method"]
topic_type:
- apiref
api_name:
- IPrinterScriptUsbJobContext.PrintedPageCount
api_type:
- COM
ms.localizationpriority: medium
---

# <span id="print.iprinterscriptusbjobcontext_printedpagecount-in"></span>IPrinterScriptUsbJobContext::PrintedPageCount method


Sets the number of pages that have been printed by the print device in the current job.

Syntax
------

```ManagedCPlusPlus
HRESULT PrintedPageCount(
  [in] UINT32 value
);
```

Parameters
----------

*value* \[in\]  
The number of pages that have been printed by the print device in the current job.

Return value
------------

This method returns an **HRESULT** value.

Remarks
-------

**PrintedPageCount** is a read/write method. The IHV JavaScript **writeData** function should keep the printed page count up to date to allow USBMon to set the correct progress on the job.

If the IHV JavaScript code never calls **PrintedPageCount** to set the printed page count, it is assumed that an accurate count of the pages is not possible and USBMon will allow the spooler to continue estimating progress.

For information about USBMon and USB-based bidirectional communication with a print device, see [USB Bidi Extender](https://msdn.microsoft.com/library/windows/hardware/jj659903).

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Minimum supported client</p></td>
<td><p>Windows 8.1</p></td>
</tr>
<tr class="even">
<td><p>Minimum supported server</p></td>
<td><p>Windows Server 2012 R2</p></td>
</tr>
<tr class="odd">
<td><p>Target platform</p></td>
<td>Desktop</td>
</tr>
</tbody>
</table>

## <span id="see_also"></span>See also


[**IPrinterScriptUsbJobContext**](iprinterscriptusbjobcontext.md)

[USB Bidi Extender](https://msdn.microsoft.com/library/windows/hardware/jj659903)

 

 




