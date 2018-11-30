---
title: licenseDetails-Ressourcentyp
description: Enthält Informationen über eine Lizenz, die einem Benutzer zugewiesen ist.
ms.openlocfilehash: dd56026d2c1d230fe6bb25b78ff8ababa01f577b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065727"
---
# <a name="licensedetails-resource-type"></a>licenseDetails-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Enthält Informationen über eine Lizenz, die einem Benutzer zugewiesen ist.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[licenseDetails auflisten](../api/user-list-licensedetails.md) | licenseDetails-Sammlung |Dient zum Abrufen einer Liste von licenseDetails-Objekten für einen Benutzer.|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Der eindeutige Bezeichner für das licenseDetails-Objekt. Schreibgeschützt, Schlüssel, lässt keine Nullwerte zu. |
|servicePlans|[servicePlanInfo](serviceplaninfo.md)-Sammlung| Informationen über die Servicepläne, die mit der Lizenz zugewiesen werden. Schreibgeschützt, lässt keine Nullwerte zu. |
|skuId|Guid| Der eindeutige Bezeichner (GUID) für die Dienst-SKU. Entspricht der skuId-Eigenschaft des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts. Schreibgeschützt |
|skuPartNumber|String| Eindeutiger SKU-Anzeigename. Entspricht der skuPartNumber des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts, z. B.: „AAD_Premium“. Schreibgeschützt |

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->