---
title: subscribedSku-Ressourcentyp
description: " Erstellen, Update und Delete werden nicht unterstützt. Abfrageausdrücke Filter werden nicht unterstützt. Erbt von directoryObject."
ms.openlocfilehash: ab9b64d8de67379aa002ffeec78edd327b15b222
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064767"
---
# <a name="subscribedsku-resource-type"></a>subscribedSku-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Für abonnierte SKUs wird nur der Lesevorgang unterstützt. Erstellen, Aktualisieren und Löschen werden nicht unterstützt. Abfragefilterausdrücke werden nicht unterstützt. Erbt von [directoryObject](directoryobject.md).


## <a name="methods"></a>Methoden
| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[subscribedSku abrufen](../api/subscribedsku-get.md) | [subscribedSku](subscribedsku.md) |Dient zum Lesen der Eigenschaften und Beziehungen des subscribedSku-Objekts.|
|[Liste subscribedsku](../api/subscribedsku-list.md) | [subscribedSku-Sammlung](subscribedsku.md) |Dienst zum Abrufen der Liste aller kommerziellen Abonnements, die eine Organisation erworben hat.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|appliesTo|String| Beispiel: „Benutzer“ oder „Community“. |
|capabilityStatus|String| Beispiel: „Aktiviert“. |
|consumedUnits|Int32| Die Anzahl der Lizenzen, die zugewiesen wurden. |
|id|String| Der eindeutige Bezeichner für das subscribedSku-Objekt. Schlüssel, lässt keine Nullwerte zu. |
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)| Informationen über die Anzahl und den Status der Prepaidlizenzen. |
|servicePlans|[servicePlanInfo](serviceplaninfo.md)-Sammlung| Informationen über die Servicepläne, die mit der SKU verfügbar sind. Lässt keine Nullwerte zu. |
|skuId|Guid| Der eindeutige Bezeichner (GUID) für die Dienst-SKU. |
|skuPartNumber|String| Die SKU-Teilenummer, z. B.: „AAD_PREMIUM“ oder „RMSBASIC“. |

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
