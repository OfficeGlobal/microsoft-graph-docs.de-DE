---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
ms.openlocfilehash: 3b2f77ea21f2352b0a8fa647af84d9b0af08a2ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058456"
---
# <a name="itemactionset-resource-type"></a>ItemActionSet-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **ItemActionSet**-Ressource enthält Informationen zu den Aktionen, die eine [Aktivität][itemActivity] zu einem Element bilden.

[itemActivity]: itemactivity.md

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka": "oneDrive.action"
}-->

```json
{
  "comment": {"@odata.type": "microsoft.graph.commentAction"},
  "create": {"@odata.type": "microsoft.graph.createAction"},
  "delete": {"@odata.type": "microsoft.graph.deleteAction"},
  "edit": {"@odata.type": "microsoft.graph.editAction"},
  "mention": {"@odata.type": "microsoft.graph.mentionAction"},
  "move": {"@odata.type": "microsoft.graph.moveAction"},
  "rename": {"@odata.type": "microsoft.graph.renameAction"},
  "restore": {"@odata.type": "microsoft.graph.restoreAction"},
  "share": {"@odata.type": "microsoft.graph.shareAction"},
  "version": {"@odata.type": "microsoft.graph.versionAction"},
  
}
```

## <a name="properties"></a>Eigenschaften

Nachstehend finden Sie die aktuell verfügbaren Aktionen.
Zukünftig werden möglicherweise neue Aktionen protokolliert, vergewissern Sie sich deshalb, ob Ihre App die Toleranz vonn **itemActionSet** ohne Aktionen unterstützt, die Ihre App versteht.

| Eigenschaftsname | Typ              | Beschreibung
|:--------------|:------------------|:-----------------------------------------
| Kommentar       | [commentAction][] | Ein Kommentar wurde zu dem Element hinzugefügt.
| create        | [createAction][]  | Ein Element wurde erstellt.
| Löschen        | [deleteAction][]  | Ein Element wurde gelöscht.
| Bearbeiten          | [editAction][]    | Ein Element wurde bearbeitet.
| Erwähnung       | [mentionAction][] | Ein Benutzer wurde im Element erwähnt.
| verschieben          | [moveAction][]    | Ein Element wurde verschoben.
| rename        | [renameAction][]  | Ein Element wurde umbenannt.
| wiederherstellen       | [restoreAction][] | Ein Element wurde wiederhergestellt.
| freigeben         | [shareAction][]   | Ein Element wurde freigegeben.
| Version       | [versionAction][] | Ein Element wurde mit einer Versionsangabe versehen.

[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a>Hinweise

Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
