---
title: Ressourcentyp deviceDetail
description: Gibt Gerätedetails zugeordnete eines Geräts zum Anmelden an. Enthält Informationen wie Gerätebrowser und Betriebssystem Info, wenn Gerät Azure AD verwaltet wird.
ms.openlocfilehash: d7c1830ee5c99fc139a937fcee3896e2a9926592
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059139"
---
# <a name="devicedetail-resource-type"></a>Ressourcentyp deviceDetail
Gibt Gerätedetails zugeordnete eines Geräts zum Anmelden an. Enthält Informationen wie Gerätebrowser und Betriebssystem Info, wenn Gerät Azure AD verwaltet wird.



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Browser|String|Gibt die Browserinformationen an der die verwendeten für die Anmeldung.|
|deviceId|String|Bezieht sich auf die UniqueID des Geräts für die Anmeldung verwendet.|
|displayName|String|Bezieht sich auf den Namen des Geräts für die Anmeldung verwendet.|
|isCompliant|Boolean|Gibt an, ob das Gerät kompatibel ist.|
|isManaged|Boolescher Wert|Gibt an, ob das Gerät oder nicht verwaltet ist.|
|operatingSystem|String|Gibt an, der Name des Betriebssystems und die Version für die Anmeldung verwendet.|
|trustType|String|Gibt an, ob das Gerät angemeldet ist Jahrestag beigetreten AzureAD beigetreten ist, ist die Domäne eingebundener Informationen. |

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