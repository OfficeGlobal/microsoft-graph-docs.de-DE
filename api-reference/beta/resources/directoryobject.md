---
title: directoryObject-Ressourcentyp
description: Stellt ein Azure Active Directory-Objekt dar. Der **directoryObject**-Typ ist der Basistyp für die meisten anderen Directory-Entitätstypen.
localization_priority: Priority
ms.openlocfilehash: a03ec966f966df556ab0122958b0b8f5464cf4fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889719"
---
# <a name="directoryobject-resource-type"></a>directoryObject-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt ein Azure Active Directory-Objekt dar. Der **directoryObject**-Typ ist der Basistyp für die meisten anderen Directory-Entitätstypen.

Diese Ressource unterstützt Folgendes:

- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/directoryobject-delta.md)-Funktion.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[directoryObject abrufen](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |Dient zum Lesen der Eigenschaften des directory-Objekts.|
|[Delete](../api/directoryobject-delete.md) | Keine |Dient zum Löschen eines directory-Objekts. |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|Zeichenfolgenauflistung|Sucht nach einer Mitgliedschaft in einer Liste von Gruppen. Die Überprüfung ist transitiv.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|Zeichenfolgenauflistung|Gibt alle Gruppen zurück, in denen das Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv.|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|Zeichenfolgenauflistung| Gibt alle Gruppen und Verzeichnisrollen zurück, in denen ein Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv. |
|[getByIds](../api/directoryobject-getbyids.md) | [directoryObject](directoryobject.md)-Sammlung | Dient zum Abrufen eines Satzes von Directory-Objekten basierend auf einem Satz angegebener IDs. |
|[validateProperties](../api/directoryobject-validateproperties.md)|JSON| Anzeigenamen ein Office 365-Gruppe zu überprüfen, oder e-Mail-Spitzname naming Richtlinien entspricht. |
|[delta](../api/directoryobject-delta.md)|directoryObject-Sammlung| Rufen Sie inkrementelle Änderungen für Directory-Objekte. Unterstützt das Filtern nach abgeleitete Typ. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|id|Zeichenfolge|Eine Guid, die den eindeutigen Bezeichner für das Objekt ist; beispielsweise 12345678-9abc-def0-1234-56789abcde12. Schlüssel. Lässt keine Nullwerte zu. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen

Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
