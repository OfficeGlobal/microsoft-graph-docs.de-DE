---
title: Ressourcentyp educationSynchronizationCustomization
description: 'Stellt Einstellungen zum Anpassen der Schule Daten profilsynchronisierung Ressource Entitäten bereit. Die Anpassung kann auf allen synchronisierten Entitäten angewendet werden. '
ms.openlocfilehash: 51799e01e5ab48fc5e686d72d2bdb5c85f191e1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059230"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>Ressourcentyp educationSynchronizationCustomization

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt Einstellungen zum Anpassen der Schule Daten profilsynchronisierung Ressource Entitäten bereit. Die Anpassung kann auf allen synchronisierten Entitäten angewendet werden. 

>**Hinweis:** Die **SynchronizationStartDate** -Eigenschaft gilt nur für die Entität **StudentEnrollment** .

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **optionalPropertiesToSync** | Auflistung der Zeichenfolge |  Die Auflistung von Eigenschaftennamen synchronisieren. Wenn auf null festgelegt, alle Eigenschaften werden synchronisiert.       |
| **synchronizationStartDate** | DateTime |  Das Datum, das die Synchronisierung gestartet werden soll. Dieser Wert sollte zu einem späteren Zeitpunkt festgelegt werden. Wenn der Wert Null, die Ressource synchronisiert werden soll, wenn das Profil Setup abgeschlossen ist. **Hinweis:** Dies gilt nur für die **StudentEnrollment** -Eigenschaft.      |
|**isSyncDeferred** |Boolesch | Gibt an, ob die Synchronisierung der übergeordneten Entität zu einem späteren Zeitpunkt verzögert ist. |
| **allowDisplayNameUpdate** | Boolesch |  Gibt an, ob der Anzeigename der Ressource durch die Synchronisierung überschrieben werden kann.         |


## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
