---
title: Ressourcentyp office365GroupsActivityStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 180e60a52b397f969aa10cee5bc27bba934ad1e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944453"
---
# <a name="office365groupsactivitystorage-resource-type"></a>Ressourcentyp office365GroupsActivityStorage

## <a name="properties"></a>Eigenschaften

| Eigenschaft                  | Typ   | Beschreibung                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Datum   | Das aktuelle Datum des Inhalts.          |
| mailboxStorageUsedInBytes | Int64  | Der Speicher, die in der Gruppenpostfach verwendet.       |
| siteStorageUsedInBytes    | Int64  | Der Speicher in SharePoint-Dokumentbibliothek verwendet wird. |
| reportDate                | Datum   | Das Datum Snapshot für Exchange und SharePoint verwendet Speicher. |
| reportPeriod              | Zeichenfolge | Die Anzahl der Tage, die der Bericht wird behandelt.    |

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
