---
title: outlookUser-Ressourcentyp
description: Stellt die für einen Benutzer verfügbaren Outlook-Dienste dar.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 32d621b71770d220487b60b4573fb34cdf28d526
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982820"
---
# <a name="outlookuser-resource-type"></a>outlookUser-Ressourcentyp


Stellt die für einen Benutzer verfügbaren Outlook-Dienste dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Kategorie erstellen](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |Erstellen eines **outlookCategory**-Objekts in der Masterliste von Kategorien.|
|[Kategorien auflisten](../api/outlookuser-list-mastercategories.md) | [outlookCategory](outlookcategory.md)-Sammlung |Ruft alle Kategorien ab, die für den Benutzer definiert wurden.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | [localeInfo](localeinfo.md)-Sammlung | Abrufen der Liste von Gebietsschemas und Sprachen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert. |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md)-Sammlung | Abrufen der Liste von Zeitzonen, die für den Benutzer unterstützt werden, wie auf dem Postfachserver des Benutzers konfiguriert. |


## <a name="properties"></a>Eigenschaften
Keine

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|masterCategories|[outlookCategory](../resources/outlookcategory.md)-Sammlung| Eine Liste von Kategorien, die für den Benutzer definiert sind. | 

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookUser",
  "@odata.annotations": [
    {
      "property": "masterCategories",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
