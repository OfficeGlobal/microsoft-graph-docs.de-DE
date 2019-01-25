---
title: Ressourcentyp educationSynchronizationError
description: Stellt einen Fehler bei der Validierung der Schule Profil und/oder Sync dar. Für jeden Eintrag, der nicht überprüfen und/oder Synchronisieren mit Azure Active Directory (AD Azure), ist ein eindeutiger Fehler generiert.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525143"
---
# <a name="educationsynchronizationerror-resource-type"></a>Ressourcentyp educationSynchronizationError

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt einen Fehler bei der Validierung der Schule Profil und/oder Sync dar. Für jeden Eintrag, der nicht überprüfen und/oder Synchronisieren mit Azure Active Directory (AD Azure), ist ein eindeutiger Fehler generiert.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-|:-|:-|
| [Abrufen von Synchronisierungsfehler](../api/educationsynchronizationerrors-get.md) | **EducationSynchronizationError** -Auflistung| Gibt die Liste der Synchronisierungsfehler im Zusammenhang mit einem Profil. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **entryType** | string |  Stellt die Sync-Entität (Schule, Abschnitt, Student, Lehrer).       |
| errorCode | string |  Stellt den Fehlercode für diesen Fehler.         |
| error.message | string |  Enthält eine Beschreibung des Fehlers.        |
| **joiningValue** | string |  Der eindeutige Bezeichner für den Eintrag.         |
| recordedDateTime | DateTimeOffset | Der Zeitpunkt des Auftretens dieses Fehlers.         |
| **reportableIdentifier** | string | Der Bezeichner für diesen Fehlereintrag.       |

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
