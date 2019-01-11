---
title: Ressourcentyp office365GroupsActivityStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 9824d3d172a8578f8a25a049c2d0d3b407bbc47e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862251"
---
# <a name="office365groupsactivitystorage-resource-type"></a>Ressourcentyp office365GroupsActivityStorage

## <a name="properties"></a>Eigenschaften

| Eigenschaft                  | Typ   | Beschreibung                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Datum   | Das aktuelle Datum des Inhalts.          |
| mailboxStorageUsedInBytes | Int64  | Der Speicher, die in der Gruppenpostfach verwendet.       |
| siteStorageUsedInBytes    | Int64  | Der Speicher in SharePoint-Dokumentbibliothek verwendet wird. |
| reportDate                | Datum   | Das Datum Snapshot für Exchange und SharePoint verwendet Speicher. |
| reportPeriod              | String | Die Anzahl der Tage, die der Bericht wird behandelt.    |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
