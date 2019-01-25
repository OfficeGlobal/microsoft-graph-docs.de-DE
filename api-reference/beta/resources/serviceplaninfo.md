---
title: servicePlanInfo-Ressourcentyp
description: Enthält Informationen zu einem Serviceplan, der einer abonnierten SKU zugeordnet ist. Die **servicePlans**-Eigenschaft der **subscribedSku**-Entität ist eine Sammlung von servicePlanInfo.
localization_priority: Normal
ms.openlocfilehash: e759082984cc66f7d3efec3cbb7cbee11561f253
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512605"
---
# <a name="serviceplaninfo-resource-type"></a>servicePlanInfo-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enthält Informationen zu einem Serviceplan, der einer abonnierten SKU zugeordnet ist. Die **servicePlans**-Eigenschaft der [subscribedSku](subscribedsku.md)-Entität ist eine Sammlung von **servicePlanInfo**.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|servicePlanId|Guid|Der eindeutige Bezeichner des Serviceplans.|
|servicePlanName|String|Der Name des Serviceplans.|
|provisioningStatus|String|Der Bereitstellungsstatus des Serviceplans. Mögliche Werte:<br/>„Success“ - Der Dienst wurde vollständig bereitgestellt.<br/>„Disabled“ - Der Dienst wurde deaktiviert.<br/>„PendingInput“ - Der Dienst wurde noch nicht bereitgestellt, es wird auf die Dienstbestätigung gewartet.<br/>"PendingActivation" - Dienst erfordert explizite Aktivierung vom Administrator (beispielsweise Intune_O365 Dienstplan) jedoch bereitgestellt wird.<br/>„PendingProvisioning“ - Microsoft hat einen neuen Dienst zur Produkt-SKU hinzugefügt, der noch nicht im Mandanten aktiviert wurde.|
|appliesTo|String|Das Objekt, dem der Serviceplan zugewiesen werden kann. Mögliche Werte:<br/>„User“ - Der Serviceplan kann einzelnen Benutzern zugewiesen werden.<br/>„Company“ - Der Serviceplan kann dem gesamten Mandanten zugewiesen werden.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/serviceplaninfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
