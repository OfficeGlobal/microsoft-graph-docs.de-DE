---
title: Location-Ressourcentyp
description: Stellt Standortinformationen eines Ereignisses dar.
localization_priority: Normal
ms.openlocfilehash: 6e3c61bcf8f22a20bf41053c2310dc51f5b800a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508608"
---
# <a name="location-resource-type"></a>Location-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| locationEmailAddress | String | Optionale E-Mail-Adresse des Orts. |
| locationUri | Zeichenfolge | Optionaler URI, der den Ort darstellt. |
| locationType | Zeichenfolge | Der Typ des Orts. Mögliche Werte sind: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`. Schreibgeschützt.|
| uniqueId | String | Nur für internen Gebrauch.|
| uniqueIdType | String | Nur für internen Gebrauch. |


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
<!--
{
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/location.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
