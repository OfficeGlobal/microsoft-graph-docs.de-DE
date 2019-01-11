---
title: Location-Ressourcentyp
description: Stellt Standortinformationen eines Ereignisses dar.
localization_priority: Normal
ms.openlocfilehash: 553634aec386798ac17e00b83883c54a99c0f9ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879800"
---
# <a name="location-resource-type"></a>Location-Ressourcentyp

Stellt Standortinformationen eines [Ereignisses](event.md) dar.

Es gibt mehrere Methoden zum Erstellen von Ereignissen in einem Kalender, z. B. über eine App mithilfe der REST-API [Ereignis erstellen](../api/user-post-events.md) oder manuell mithilfe der Outlook-Benutzeroberfläche. Wenn Sie ein Ereignis über die Benutzeroberfläche erstellen, können Sie den Ort als Nur-Text angeben (z. B. „Harrys Bar“) oder aus der in Outlook bereitgestellten Raumliste, [Bing-Vorschlagssuche](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) oder [lokale Bing-Suche](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/). 

Je nachdem, wie ein Ereignis erstellt wurde, wird die schreibgeschützte **locationType**-Eigenschaft anders festgelegt. 

| Wie ein Ereignis erstellt wurde  | Eigenschaft   | Erwarteter Wert |
|:----------|:-------|:--------------------------------|
| REST-API [Ereignis erstellen](../api/user-post-events.md)  | **locationType** | `default` |
| Benutzeroberfläche in Outlook | **locationType** | Eine der folgenden Varianten: <ul><li>`default` für einen Ort, der als Nur-Text eingegeben wird.</li><li>`conferenceRoom` für einen Raum, der von der Outlook-Raumliste bereitgestellt wird.</li><li>Oder eine der folgenden Listen – `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` – für einen Ort aus der Bing-Vorschlagssuche oder der lokalen Bing-Suche.</li></ul> |

## <a name="properties"></a>Eigenschaften
| Eigenschaft  | Typ   | Beschreibung                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| address | [physicalAddress](physicaladdress.md) |Die Adresse des Orts. |
| Koordinaten | [outlookGeoCoordinates](outlookgeocoordinates.md) | Die geografischen Koordinaten und die Erhebung des Orts. |
| displayName  | String | Der Name, der mit dem Ort verknüpft ist                       |
| locationEmailAddress | String | Optionale E-Mail-Adresse des Orts.              |
| locationUri | String | Optionaler URI, der den Ort darstellt. |
| locationType | locationType | Der Typ des Orts. Die möglichen Werte sind: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`. Schreibgeschützt.|
| uniqueId | String | Nur für internen Gebrauch.|
| uniqueIdType | locationUniqueIdType | Nur für internen Gebrauch. |

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string",
  "locationType": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
