---
title: " Ressourcentyp averageComparativeScore"
description: Diese Ressource enthält verschiedene unterschiedliche Faktoren, die von unterschiedlichen Bereichen (beispielsweise Durchschnitt von Branche vertikal, durchschnittliche vom Unternehmen Arbeitsplatz Größe usw.) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) basiert.
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834594"
---
#  <a name="averagecomparativescore-resource-type"></a>Ressourcentyp averageComparativeScore

Diese Ressource enthält verschiedene unterschiedliche Faktoren, die von unterschiedlichen Bereichen (beispielsweise Durchschnitt von Branche vertikal, durchschnittliche vom Unternehmen Arbeitsplatz Größe usw.) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) basiert.

|Eigenschaft |Typ |Beschreibung |
|:--|:--|:--|
|   Basis   |   Zeichenfolge  |   Typ des Gültigkeitsbereichs (durch AllTenants TotalSeats, IndustryTypes).  |
|   averageScore    |   Gleitkommawert mit doppelter Genauigkeit  | Durchschnittliche Punktzahl innerhalb der angegebenen Basis. |
|   deviceScore |   Gleitkommawert mit doppelter Genauigkeit  | Durchschnittliche Punktzahl innerhalb der angegebenen Basis. |
|   dataScore   |   Gleitkommawert mit doppelter Genauigkeit  | Durchschnittliche Punktzahl innerhalb der angegebenen Basis. |
|   identityScore   |   Gleitkommawert mit doppelter Genauigkeit  | Durchschnittliche Punktzahl innerhalb der angegebenen Basis. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double",
  "deviceScore": "Double",
  "dataScore": "Double",
  "identityScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
