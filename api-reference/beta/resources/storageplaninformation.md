---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: bbe4faaffbf53c24d4d0f5b8ea1f5ee1e1966a2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860123"
---
# <a name="storageplaninformation-resource-type"></a>Ressourcentyp storagePlanInformation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **StoragePlanInformation** Ressource enthält Informationen über das Laufwerk Speicherung Kontingent Pläne.

### <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```
## <a name="properties"></a>Eigenschaften

| Eigenschaftenname     | Typ      | Beschreibung                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| upgradeAvailable  | Boolean   | Gibt an, ob einer höheren Speicherung Kontingent Plänen verfügbar sind. Schreibgeschützt. |


<!-- {
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation"
} -->

