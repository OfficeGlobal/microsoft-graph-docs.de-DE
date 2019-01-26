---
title: Ressourcentyp office365GroupsActivityStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576381"
---
# <a name="office365groupsactivitystorage-resource-type"></a>Ressourcentyp office365GroupsActivityStorage

## <a name="properties"></a>Eigenschaften

| Eigenschaft                  | Typ   | Beschreibung                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Date   | Das aktuelle Datum des Inhalts.          |
| mailboxStorageUsedInBytes | Int64  | Der Speicher, die in der Gruppenpostfach verwendet.       |
| siteStorageUsedInBytes    | Int64  | Der Speicher in SharePoint-Dokumentbibliothek verwendet wird. |
| reportDate                | Date   | Das Datum Snapshot für Exchange und SharePoint verwendet Speicher. |
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
