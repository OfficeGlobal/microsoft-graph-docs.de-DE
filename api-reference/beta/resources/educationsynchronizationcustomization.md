---
title: Ressourcentyp educationSynchronizationCustomization
description: 'Stellt Einstellungen zum Anpassen der Schule Daten profilsynchronisierung Ressource Entitäten bereit. Die Anpassung kann auf allen synchronisierten Entitäten angewendet werden. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513606"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>Ressourcentyp educationSynchronizationCustomization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt Einstellungen zum Anpassen der Schule Daten profilsynchronisierung Ressource Entitäten bereit. Die Anpassung kann auf allen synchronisierten Entitäten angewendet werden. 

>**Hinweis:** Die **SynchronizationStartDate** -Eigenschaft gilt nur für die Entität **StudentEnrollment** .

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **optionalPropertiesToSync** | Collection of String
 |  Die Auflistung von Eigenschaftennamen synchronisieren. Wenn auf null festgelegt, alle Eigenschaften werden synchronisiert.       |
| **synchronizationStartDate** | DateTime |  Das Datum, das die Synchronisierung gestartet werden soll. Dieser Wert sollte zu einem späteren Zeitpunkt festgelegt werden. Wenn der Wert Null, die Ressource synchronisiert werden soll, wenn das Profil Setup abgeschlossen ist. **Hinweis:** Dies gilt nur für die **StudentEnrollment** -Eigenschaft.      |
|**isSyncDeferred** |Boolescher Wert | Gibt an, ob die Synchronisierung der übergeordneten Entität zu einem späteren Zeitpunkt verzögert ist. |
| **allowDisplayNameUpdate** | Boolescher Wert |  Gibt an, ob der Anzeigename der Ressource durch die Synchronisierung überschrieben werden kann.         |


## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
