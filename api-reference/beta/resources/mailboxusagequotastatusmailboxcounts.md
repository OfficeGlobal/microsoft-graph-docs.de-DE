---
title: Ressourcentyp mailboxUsageQuotaStatusMailboxCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45e4754fef0dd3a2f7a669e3b3b96692d117c8f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921234"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>Ressourcentyp mailboxUsageQuotaStatusMailboxCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ   |
| :-------------------- | :----- |
| reportRefreshDate     | Datum   |
| underLimit            | Int64  |
| warningIssued         | Int64  |
| sendProhibited        | Int64  |
| sendReceiveProhibited | Int64  |
| unbestimmten         | Int64  |
| reportDate            | Datum   |
| reportPeriod          | Zeichenfolge |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "underLimit": 1024, 
  "warningIssued": 1024, 
  "sendProhibited": 1024, 
  "sendReceiveProhibited": 1024, 
  "indeterminate": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
