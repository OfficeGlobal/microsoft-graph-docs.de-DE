---
title: directory-Ressourcentyp (Gelöschte Elemente)
description: . Ein kürzlich gelöschtes Element kann bis zu 30 Tage lang wiederhergestellt werden. Nach 30 Tagen wird das Element dauerhaft gelöscht.
localization_priority: Normal
ms.openlocfilehash: e8ccecfd0d8cffa383ecc96cc908d31452db5fb0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835770"
---
# <a name="directory-resource-type-deleted-items"></a>directory-Ressourcentyp (Gelöschte Elemente)

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

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|deletedItems|[directoryObject](directoryobject.md)-Sammlung| Kürzlich gelöschte Elemente. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a>Beispiel

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
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
