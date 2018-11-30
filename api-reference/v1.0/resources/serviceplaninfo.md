---
title: servicePlanInfo-Ressourcentyp
description: Enthält Informationen zu einem Serviceplan, der einer abonnierten SKU zugeordnet ist. Die **servicePlans**-Eigenschaft der subscribedSku-Entität ist eine Sammlung von **servicePlanInfo**.
ms.openlocfilehash: 70d49eb22542e9bc22ee28df5bc77b3bf6146b6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017896"
---
# <a name="serviceplaninfo-resource-type"></a>servicePlanInfo-Ressourcentyp

Enthält Informationen zu einem Serviceplan, der einer abonnierten SKU zugeordnet ist. Die **servicePlans**-Eigenschaft der [subscribedSku](subscribedsku.md)-Entität ist eine Sammlung von **servicePlanInfo**.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|servicePlanId|Guid|Der eindeutige Bezeichner des Serviceplans.|
|servicePlanName|String|Der Name des Serviceplans.|
|provisioningStatus|String|Der Bereitstellungsstatus des Serviceplans. Mögliche Werte:<br/>„Success“ - Der Dienst wurde vollständig bereitgestellt.<br/>„Disabled“ - Der Dienst wurde deaktiviert.<br/>„PendingInput“ - Der Dienst wurde noch nicht bereitgestellt, es wird auf die Dienstbestätigung gewartet.<br/>„PendingActivation“ - Der Dienst wurde bereitgestellt, erfordert aber die explizite Aktivierung durch einen Administrator (z. B. Intune_O365-Serviceplan)<br/>„PendingProvisioning“ - Microsoft hat einen neuen Dienst zur Produkt-SKU hinzugefügt, der noch nicht im Mandanten aktiviert wurde.|
|appliesTo|Zeichenfolge|Das Objekt, dem der Serviceplan zugewiesen werden kann. Mögliche Werte:<br/>„User“ - Der Serviceplan kann einzelnen Benutzern zugewiesen werden.<br/>„Company“ - Der Serviceplan kann dem gesamten Mandanten zugewiesen werden.|

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
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
