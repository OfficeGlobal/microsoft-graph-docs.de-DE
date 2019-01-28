---
title: directoryObject-Ressourcentyp
description: Stellt ein Azure Active Directory-Objekt dar. Der **directoryObject**-Typ ist der Basistyp für die meisten anderen Directory-Entitätstypen.
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ba2454a5eda90ec50dbd6a0c152383bb42a437d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573956"
---
# <a name="directoryobject-resource-type"></a>directoryObject-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt ein Azure Active Directory-Objekt dar. Der **directoryObject**-Typ ist der Basistyp für die meisten anderen Directory-Entitätstypen.

Diese Ressource unterstützt Folgendes:

- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/directoryobject-delta.md)-Funktion.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[directoryObject abrufen](../api/directoryobject-get.md) | [directoryObject](../resources/directoryobject.md) |Dient zum Lesen der Eigenschaften des directory-Objekts.|
|[Delete](../api/directoryobject-delete.md) | Keine |Dient zum Löschen eines directory-Objekts. |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|String collection|Sucht nach einer Mitgliedschaft in einer Liste von Gruppen. Die Überprüfung ist transitiv.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|String collection|Gibt alle Gruppen zurück, in denen das Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv.|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String collection| Gibt alle Gruppen und Verzeichnisrollen zurück, in denen ein Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Die Überprüfung ist transitiv. |
|[getByIds](../api/directoryobject-getbyids.md) | [directoryObject](../resources/directoryobject.md)-Sammlung | Dient zum Abrufen eines Satzes von Directory-Objekten basierend auf einem Satz angegebener IDs. |
|[validateProperties](../api/directoryobject-validateproperties.md)|JSON| Überprüft, ob der Anzeigename oder E-Mail-Kontoname einer Office 365-Gruppe den Benennungsrichtlinien entspricht. |
|[delta](../api/directoryobject-delta.md)|directoryObject-Sammlung| Abrufen inkrementeller Änderungen für Verzeichnisobjekte. Unterstützt das Filtern nach abgeleitetem Typ. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|id|String|Eine GUID, die der eindeutige Bezeichner für das Objekt ist, z. B. 12345678-9abc-def0-1234-56789abcde12. Schlüssel. Lässt keine Nullwerte zu. Schreibgeschützt.|

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
