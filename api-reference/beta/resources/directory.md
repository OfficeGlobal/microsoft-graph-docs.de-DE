---
title: directory-Ressourcentyp (Gelöschte Elemente)
description: . Ein kürzlich gelöschtes Element kann bis zu 30 Tage lang wiederhergestellt werden. Nach 30 Tagen wird das Element dauerhaft gelöscht.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2593603afa145d30b5e26a240bb5cd471eab9942
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966552"
---
# <a name="directory-resource-type-deleted-items"></a>directory-Ressourcentyp (Gelöschte Elemente)

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt ein gelöschtes Element im Verzeichnis dar. Wenn ein Element gelöscht wird, wird es dem Container „Gelöschte Elemente“ hinzugefügt. Ein kürzlich gelöschtes Element kann bis zu 30 Tage lang wiederhergestellt werden. Nach 30 Tagen wird das Element dauerhaft gelöscht.

Die Funktion für gelöschte Elemente wird derzeit nur für die Office 365-Ressourcen [group](group.md) und [user](users.md) unterstützt.

## <a name="methods"></a>Methoden

| Methode         | Rückgabetyp | Beschreibung |
|:---------------|:------------|:------------|
|[Gelöschtes Element abrufen](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Ruft die Eigenschaften eines gelöschten Elements ab. |
|[Gelöschtes Element wiederherstellen](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| Stellt ein kürzlich gelöschtes Element wieder her. |
|[Gelöschte Elemente auflisten](../api/directory-deleteditems-list.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft eine Liste der kürzlich gelöschten Elemente ab. |
|[Element endgültig löschen](../api/directory-deleteditems-delete.md) | Keine | Löscht ein Element endgültig. |
|[Gelöschte Listenelemente Besitz eines Benutzers](../api/directory-deleteditems-user-owned.md) | [directoryObject](directoryobject.md)-Sammlung | Enthält Directory Elemente, die einem Benutzer gehören. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|id|Zeichenfolge| Ein eindeutiger Bezeichner für das Objekt, z. B. 12345678-9abc-def0-1234-56789abcde. Schlüssel. Lässt keine Nullwerte zu. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|deleteditems|[directoryObject](directoryobject.md)-Sammlung| Kürzlich gelöschte Elemente. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
