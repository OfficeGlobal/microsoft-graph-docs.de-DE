---
title: Ressourcentyp deviceDetail
description: Gibt Gerätedetails zugeordnete eines Geräts zum Anmelden an. Enthält Informationen wie Gerätebrowser und Betriebssystem Info, wenn Gerät Azure AD verwaltet wird.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18d55e397cf6c892cd37aea930d446c630017a92
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971361"
---
# <a name="devicedetail-resource-type"></a>Ressourcentyp deviceDetail
Gibt Gerätedetails zugeordnete eines Geräts zum Anmelden an. Enthält Informationen wie Gerätebrowser und Betriebssystem Info, wenn Gerät Azure AD verwaltet wird.



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Browser|Zeichenfolge|Gibt die Browserinformationen an der die verwendeten für die Anmeldung.|
|deviceId|Zeichenfolge|Bezieht sich auf die UniqueID des Geräts für die Anmeldung verwendet.|
|displayName|Zeichenfolge|Bezieht sich auf den Namen des Geräts für die Anmeldung verwendet.|
|isCompliant|Boolean|Gibt an, ob das Gerät kompatibel ist.|
|isManaged|Boolescher Wert|Gibt an, ob das Gerät oder nicht verwaltet ist.|
|operatingSystem|Zeichenfolge|Gibt an, der Name des Betriebssystems und die Version für die Anmeldung verwendet.|
|trustType|Zeichenfolge|Gibt an, ob das Gerät angemeldet ist Jahrestag beigetreten AzureAD beigetreten ist, ist die Domäne eingebundener Informationen. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
