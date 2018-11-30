---
title: " Ressourcentyp averageComparativeScore"
description: Diese Ressource enthält verschiedene unterschiedliche Faktoren, die von unterschiedlichen Bereichen (beispielsweise Durchschnitt von Branche vertikal, durchschnittliche vom Unternehmen Arbeitsplatz Größe usw.) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) basiert.
ms.openlocfilehash: 08e4ec60788b21476d8f1491ab5548c7a4ca2e01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059442"
---
#  <a name="averagecomparativescore-resource-type"></a>Ressourcentyp averageComparativeScore

Diese Ressource enthält verschiedene unterschiedliche Faktoren, die von unterschiedlichen Bereichen (beispielsweise Durchschnitt von Branche vertikal, durchschnittliche vom Unternehmen Arbeitsplatz Größe usw.) und Steuerelement Kategorie (Identität, Daten, Gerät, Apps, Infrastruktur) basiert.

|Eigenschaft |Typ |Beschreibung |
|:--|:--|:--|
|   Basis   |   String  |   Typ des Gültigkeitsbereichs (durch AllTenants TotalSeats, IndustryTypes).  |
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
