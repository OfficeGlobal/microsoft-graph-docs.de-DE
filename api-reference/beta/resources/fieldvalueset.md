---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
ms.openlocfilehash: ed10b586ee55ccd32e81b03bdc6359ee13605877
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480166"
---
# <a name="fieldvalueset-resource"></a>FieldValueSet-Ressource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die Spaltenwerte in einer [ListItem](listitem.md)-Ressource dar.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **fieldValueSet**-Ressource.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
       "keyProperty": "id", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a>Eigenschaften

Jedes für den Benutzer sichtbare Feld im **ListItem** wird als Name-Wert-Paar im **FieldValueSet** wiedergegeben.
Das Beispiel oben bezieht sich auf eine Liste mit den vier Spalten **Autor**, **Namen**, **Farbe** und **Menge**.

Nachschlage-Feldern (wie `Author` oben) werden standardmäßig nicht zurückgegeben.
In diesem Fall gibt der Server ein Feld 'LookupId' (wie `AuthorLookupId` oben) zurück, das sich auf das in der Suche angegebene ListItem bezieht.
Der Name des Felds 'LookupId' besteht aus dem ursprünglichen Feldnamen gefolgt von `LookupId`.

Bis zu 12 Nachschlagetabellen in einer einzigen Abfrage angefordert werden.
Der Server gibt Nachschlagewerte zurück, wenn Ihre Anforderung eine `select`-Anweisung mit den von Ihnen benötigten Feldern enthält.
Beispiel:

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

Sie können bis zu 12 Nachschlage-Felder in einer Abfrage sowie eine beliebige Anzahl regulärer Felder anfordern.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/fieldvalueset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
