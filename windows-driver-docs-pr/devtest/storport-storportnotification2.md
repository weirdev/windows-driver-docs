---
title: StorPortNotification2 rule (storport)
description: This rule verifies that calls to StorPortNotification use only allowed (i.e. documented) notification types.
ms.assetid: 74363E6D-1D1B-484D-A558-8996DFE02FA8
ms.date: 05/21/2018
keywords: ["StorPortNotification2 rule (storport)"]
topic_type:
- apiref
api_name:
- StorPortNotification2
api_type:
- NA
ms.localizationpriority: medium
---

# StorPortNotification2 rule (storport)


This rule verifies that calls to **StorPortNotification** use only allowed (i.e. documented) notification types.

The allowed notification types are:

**BufferOverrunDetected**
**BusChangeDetected**
**LinkDown**
**LinkUp**
**QueryTickCount**
**RequestComplete**
**RequestTimerCall**
**ResetDetected**
**WMIEvent**
**WMIReregister**

|              |          |
|--------------|----------|
| Driver model | Storport |

How to test
-----------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">At compile time</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Run <a href="https://msdn.microsoft.com/library/windows/hardware/ff552808" data-raw-source="[Static Driver Verifier](https://msdn.microsoft.com/library/windows/hardware/ff552808)">Static Driver Verifier</a> and specify the <strong>StorPortNotification2</strong> rule.</p>
Use the following steps to run an analysis of your code:
<ol>
<li><a href="https://msdn.microsoft.com/library/windows/hardware/hh454281#preparing-your-source-code" data-raw-source="[Prepare your code (use role type declarations).](https://msdn.microsoft.com/library/windows/hardware/hh454281#preparing-your-source-code)">Prepare your code (use role type declarations).</a></li>
<li><a href="https://msdn.microsoft.com/library/windows/hardware/hh454281#running-static-driver-verifier" data-raw-source="[Run Static Driver Verifier.](https://msdn.microsoft.com/library/windows/hardware/hh454281#running-static-driver-verifier)">Run Static Driver Verifier.</a></li>
<li><a href="https://msdn.microsoft.com/library/windows/hardware/hh454281#viewing-and-analyzing-the-results" data-raw-source="[View and analyze the results.](https://msdn.microsoft.com/library/windows/hardware/hh454281#viewing-and-analyzing-the-results)">View and analyze the results.</a></li>
</ol>
<p>For more information, see <a href="https://msdn.microsoft.com/library/windows/hardware/hh454281" data-raw-source="[Using Static Driver Verifier to Find Defects in Drivers](https://msdn.microsoft.com/library/windows/hardware/hh454281)">Using Static Driver Verifier to Find Defects in Drivers</a>.</p></td>
</tr>
</tbody>
</table>

Applies to
----------

[**StorPortNotification**](https://msdn.microsoft.com/library/windows/hardware/ff567433)








