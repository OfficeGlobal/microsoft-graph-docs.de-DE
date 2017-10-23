---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ItemReference
ms.openlocfilehash: abd8b438e6c4e364a7a4b010d0808255425fa4df
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="itemreference-resource-type"></a>ItemReference-Ressourcentyp

Die **ItemReference**-Ressource enthält Informationen, die erforderlich sind, um ein [DriveItem](driveitem.md) über die API zu adressieren.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "driveType": "personal | business | documentLibrary",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ              | Beschreibung
|:--------------|:------------------|:-----------------------------------------
| driveId       | String            | Eindeutiger Bezeichner der drive-Instanz, die das Element enthält. Schreibgeschützt.
| driveType     | Zeichenfolge            | Identifiziert den Laufwerkstyp. Werte finden Sie unter [drive][]-Ressource.
| id            | String            | Eindeutiger Bezeichner des Elements im Laufwerk. Schreibgeschützt.
| name          | Zeichenfolge            | Der Name des Elements, auf das verwiesen wird. Schreibgeschützt.
| Pfad          | String            | Pfad, der verwendet werden kann, um zu dem Element zu navigieren. Schreibgeschützt.
| shareId       | String            | Ein eindeutiger Bezeichner für eine freigegebene Ressource, auf die über [Freigabe][]-API zugegriffen werden kann.
| sharepointIds | [sharepointIds][] | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares_get.md

## <a name="remarks"></a>Hinweise

Um ein **driveItem**-Element aus einer **itemReference**-Ressource zu adressieren, erstellen Sie eine URL im folgenden Format:

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

Der **path**-Wert ist ein API-Pfad relativ zu dem Ziellaufwerk, z. B.: `/drive/root:/Documents/myfile.docx`.

Um den lesbaren Pfad für ein Breadcrumb abzurufen, können Sie alles bis zum ersten `:` in der Pfadzeichenfolge problemlos ignorieren.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "tocPath": "Resources/ItemReference"
} -->
