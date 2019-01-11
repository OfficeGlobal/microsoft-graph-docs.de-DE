---
title: Ressourcentyp mailSearchFolder
description: Ein MailSearchFolder ist ein virtueller Ordner im Postfach des Benutzers, das alle angegebenen Suchkriterien e-Mail-Elemente enthält. MailSearchFolder erbt vom MailFolder.
localization_priority: Normal
ms.openlocfilehash: 62d4d8569977c99690e317a39a43bbc9d9dca3f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870392"
---
# <a name="mailsearchfolder-resource-type"></a>Ressourcentyp mailSearchFolder

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein MailSearchFolder ist ein virtueller Ordner im Postfach des Benutzers, das alle angegebenen Suchkriterien e-Mail-Elemente enthält. MailSearchFolder erbt vom [MailFolder](mailfolder.md).

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp  | Beschreibung |
|:---------------|:--------|:----------|
| [Erstellen eines Suchordners](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | Erstellen eines Suchordners im Postfach des Benutzers an. |
| [Liste Suchordner](../api/mailfolder-list-childfolders.md) | [mailFolder](mailfolder.md)-Sammlung | Listen Sie alle Ordner im Postfach dieses Benutzers, einschließlich Suchordner. |
| [Abrufen von Ordnern suchen](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | Rufen Sie den angegebenen Suchordner. |
| [Aktualisieren eines Suchordners](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | Aktualisieren Sie den angegebenen Suchordner. |
| [Löschen eines Suchordners](../api/mailfolder-delete.md) | Keine | Löschen Sie den angegebenen Suchordner. |
| [Listen Sie alle Nachrichten in einem Suchordner](../api/mailfolder-list-messages.md) | [message](message.md)-Sammlung | Listen Sie alle Nachrichten in den angegebenen Suchordner. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
| isSupported | Boolescher Wert | Gibt an, ob ein Suchordner mithilfe von REST-APIs bearbeitet werden. |
| includeNestedFolders | Boolescher Wert | Gibt an, wie die Hierarchie der Postfach-Ordner durchlaufen werden soll. `true`bedeutet, dass eine umfassende Suche sollte erledigen `false` bedeutet, dass eine flache Suche sollte stattdessen durchgeführt werden. |
| sourceFolderIDs | Collection von Objekten des Typs „String“ | Die Postfachordner, die durchsucht werden soll. |
| filterQuery | Zeichenfolge | Der OData-Abfrage Nachrichten gefiltert werden soll. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
