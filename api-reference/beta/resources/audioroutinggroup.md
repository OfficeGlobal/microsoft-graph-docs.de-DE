---
title: Ressourcentyp audioRoutingGroup
description: Die audio Routinggruppe speichert eine private audio Route zwischen Teilnehmer an einer Unterhaltung mit mehreren Teilnehmern. Quelle der Teilnehmer selbst und die Empfänger sind eine Teilmenge der andere Teilnehmer an der Unterhaltung mit mehreren Teilnehmern.
author: VinodRavichandran
ms.openlocfilehash: 0e1db47963576e728a07a6b99ecff09a0f4640d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344471"
---
# <a name="audioroutinggroup-resource-type"></a>Ressourcentyp audioRoutingGroup

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die audio Routinggruppe speichert eine private audio Route zwischen Teilnehmer an einer Unterhaltung mit mehreren Teilnehmern. Quelle der Teilnehmer selbst und die Empfänger sind eine Teilmenge der andere Teilnehmer an der Unterhaltung mit mehreren Teilnehmern.

> **Hinweis:** [ConfigureMixer](../api/participant-configuremixer.md) beinhaltet alle Routen jedoch nicht, ist es für den gesamten Anruf zum Festlegen der Lautstärke für Source-Receiver Kombinationen aus.

## <a name="methods"></a>Methoden

| Methode                                                  | Rückgabetyp                               | Beschreibung                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [Abrufen von audioRoutingGroup](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | Lesen Sie Eigenschaften und Beziehungen des AudioRoutingGroup-Objekts.|
| [Update](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | Aktualisieren Sie Ereignisempfänger Liste.                       |
| [Delete](../api/audioroutinggroup-delete.md)            | Keine                                      | Löschen der audio Routinggruppe.              |

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ              | Beschreibung                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | String            | Schreibgeschützt. Server generiert wurde.                                         |
| Ereignisempfänger     | Zeichenfolgenauflistung | Liste der Teilnehmer Ids empfangen.                                   |
| routingMode   | String            | Routing Group-Modus.  Mögliche Werte sind: `oneToOne` und `multicast`.   |
| sources       | Zeichenfolgenauflistung | Liste der Teilnehmer Source-Ids.                                      |

> **Hinweis:** Routing Modus bestimmt die Einschränkungen auf die Quellen und Ereignisempfänger. Die folgenden Routinggruppen werden unterstützt.
> - `oneToOne`-Quellen und Ereignisempfänger nur an einen Teilnehmer haben.
> - `multicast`-Quelle ein Teilnehmer hat, aber es gibt mehrere Empfänger. Ereignisempfänger möglicherweise aktualisiert werden.

> **Hinweis:** Wenn Sie viele Audio-Routinggruppen (z. B. Bot pro Teilnehmer) erstellen, wird nur die Audiodaten der oberen 4 dominanten Lautsprecher weitergeleitet. Sie bedeutet, dass selbst bei angepassten audio Routinggruppe ist der Lautsprecher nicht laut genug im Hauptfenster Mixer, er den Robot hören, ist nicht möglich, auch wenn eine private audio Gruppe nur für diese Lautsprecher und den Robot vorhanden ist.

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "String" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "String" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
