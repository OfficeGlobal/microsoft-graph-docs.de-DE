---
title: Ressourcentyp office365GroupsActivityStorage
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 23ff4d112373f52c4c19d6631ac89bac22399b29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064924"
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
