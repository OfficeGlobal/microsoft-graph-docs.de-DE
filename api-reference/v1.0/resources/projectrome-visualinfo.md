---
title: Ressourcentyp visualInfo
description: Einen komplexen Typ für die **VisualElements** -Eigenschaft im Aktivitätsobjekt darstellt.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 416109bb1bb6625330ddfbbb32b8fb688b223134
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962646"
---
# <a name="visualinfo-resource-type"></a>Ressourcentyp visualInfo

Einen komplexen Typ für die **VisualElements** -Eigenschaft im [Aktivität](../resources/projectrome-activity.md) -Objekt darstellt.

Jede Aktivität des Benutzers werden in Zeitachse wie eine Adaptive Karte angezeigt. App-Entwickler werden empfohlen, eine benutzerdefinierte Karte angeben, die das Wesentliche der Aktivität erfasst wird, die in Ihrer app durchgeführt wurde. Dies ist möglich, durch die Bereitstellung einer benutzerdefinierten JSON-Karte in die Content-Eigenschaft.

Neben visual Metadaten mit einer Adaptive Karte app Content-Metadaten – Daten, die angeben, verwendet, um Rückschlüsse auf die Aktivität des Benutzers zu erstellen, um neue Aktivitäten für zukünftige erneute Engagements anbieten. Dies ist möglich, mithilfe der Eigenschaft der Aktivität ContentInfo dar, ein JSON-Objekt anzugeben, der schema.org-Eigenschaften, um den Inhalt beschreiben nutzt.

Wenn eine benutzerdefinierte Karte nicht angegeben ist, wird eine einfache Karte mit Anzeigetext und Beschreibungseigenschaften generiert. Benutzerdefinierte Karten werden empfohlen, um die besten Inhalte aus Ihrer App zu präsentieren.

## <a name="properties"></a>Eigenschaften

|Name | Typ | Beschreibung|
|:----|:------|:-----------|
|Anzeigetext | Zeichenfolge | Erforderlich. Kurze Beschreibung des Benutzers eindeutige Aktivität (beispielsweise Dokumentname in Fällen, in dem eine Aktivität zum Erstellen eines Dokuments bezieht sich)|
|description | Zeichenfolge | Optional. Längere Beschreibung des eindeutigen Benutzeraktivität (Beispiel: Dokument-Namen, den ersten Satz und/oder Metadaten)|
|backgroundColor | Zeichenfolge | Optional. Hintergrundfarbe verwendet, um die Aktivität in der UI - Marke Farbe für die Anwendungsquelle der Aktivität zu rendern. Muss eine gültige hex Farbe|
|content | Nicht typisierte JSON-Objekt | Optional. Benutzerdefinierte Datenelement - JSON-Objekt verwendet, um benutzerdefinierte Inhalte für die Aktivität in der Windows-Shell UI Rendern bereitstellen|
|Zuweisung | [imageInfo](../resources/projectrome-imageinfo.md) | Optional. JSON-Objekt verwendet, um ein Symbol darstellen, die die Anwendung verwendet, um die Aktivität generieren darstellt|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
