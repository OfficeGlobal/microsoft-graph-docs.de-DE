---
title: GetNamedItem Ressourcenart
description: Stellt einen definierten Namen für einen Zellbereich oder einen Wert dar. Namen können einfach benannte Objekte (wie unten dargestellt), Bereichsobjekte, Verweise auf einen Bereich sein. Dieses Objekt kann zum Abrufen des mit Namen verknüpften Bereichsobjekts verwendet werden.
ms.openlocfilehash: 11ca12e0ae094f0e682cfde5fb1fe1feecabdb9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061830"
---
# <a name="nameditem-resource-type"></a>GetNamedItem Ressourcenart

Stellt einen definierten Namen für einen Zellbereich oder einen Wert dar. Namen können einfach benannte Objekte (wie unten dargestellt), Bereichsobjekte, Verweise auf einen Bereich sein. Dieses Objekt kann zum Abrufen des mit Namen verknüpften Bereichsobjekts verwendet werden.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Add](../api/nameditem-add.md)|[NamedItem](nameditem.md)|Fügt einen neuen Namen zur Auflistung des angegebenen Bereichs hinzu.|
|[AddFormulaLocal](../api/nameditem-addformulalocal.md)|[NamedItem](nameditem.md)|Fügt unter Verwendung des Gebietsschemas des Benutzers für die Formel einen neuen Namen zur Auflistung des angegebenen Bereichs hinzu.|
|[NamedItem abrufen](../api/nameditem-get.md) | [NamedItem](nameditem.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des namedItem-Objekts.|
|[Update](../api/nameditem-update.md) | [NamedItem](nameditem.md)   |Dient zum Aktualisieren des NamedItem-Objekts. |
|[Range](../api/nameditem-range.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit dem Namen verknüpft ist. Gibt eine Ausnahme zurück, wenn der Typ des benannten Elements kein Bereich ist.|
|[List](../api/nameditem-list.md) | [NamedItem-Sammlung](nameditem.md) |Dient zum Abrufen einer der namedItem-Objektsammlung. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|name|string|Der Name des Objekts. Schreibgeschützt.|
|comment|string|Stellt den Kommentar dar, der mit diesem Namen verknüpft ist.|
|scope|string|Gibt an, ob der Name im Bereich der Arbeitsmappe oder im Bereich eines bestimmten Arbeitsblatts liegt. Schreibgeschützt.|
|type|string|Gibt an, welche Art von Verweis mit dem Namen verknüpft ist. Mögliche Werte:`String`, `Integer`, `Double`, `Boolean`, `Range`. Schreibgeschützt.|
|Wert|string|Stellt die Formel dar, auf die der Name verweist. z. B. =Sheet14!$B$2:$H$12, =4.75 usw. Schreibgeschützt.|
|visible|boolean|Gibt an, ob das Objekt sichtbar ist.|

## <a name="relationships"></a>Beziehungen
| Beziehung     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Arbeitsblatt|[worksheet](worksheet.md)|Gibt das Arbeitsblatt zurück, auf dessen Bereich das benannte Element beschränkt ist. Nur verfügbar, wenn das Element auf das Arbeitsblatt beschränkt ist. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": "string",
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
