---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
ms.openlocfilehash: 7c8cdab7adc705333d1aeaad526aeeb813de10a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064499"
---
# <a name="itemactivity-resource-type"></a>ItemActivity-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **ItemActivity**-Ressource stellt Informationen zu Aktivitäten bereit, die zu einem Element oder innerhalb eines Containers stattfanden.
Zurzeit nur für SharePoint und OneDrive for Business verfügbar.

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivity",
  "@type.aka": "oneDrive.activityEntity"
}-->

```json
{
  "id": "string (identifier)",
  "access": "microsoft.graph.accessAction",
  "action": {"@odata.type": "microsoft.graph.itemActionSet"},
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "location": {"@odata.type": "microsoft.graph.location"},
  "times": {"@odata.type": "microsoft.graph.itemActivityTimeSet"}
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ                    | Beschreibung
|:---------|:------------------------|:----------------------------------------
| id       | string                  | Der eindeutige Bezeichner der Aktivität. Schreibgeschützt.
| Zugriff   | [accessAction][]        | Ein Element wurde zugegriffen.
| Aktion   | [itemActionSet][]       | Details zu der Aktion, die durchgeführt wurde. Schreibgeschützt.
| Akteur    | [identitySet][]         | Die Identität der Person, die die Aktion ausgeführt hat. Schreibgeschützt.
| location | [location][]            | Physischen Standort, auf dem die Aktion ausgeführt wurde. Schreibgeschützt.
| Mal    | [itemActivityTimeSet][] | Details zum Zeitpunkt der Ausführung der Aktivität. Schreibgeschützt.

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a>Beziehungen

| Beziehungsname | Typ          | Beschreibung
|:------------------|:--------------|:-----------------------------------------
| driveItem         | [driveItem][] | Macht das **DriveItem** verfügbar, das Ziel dieser Aktivität war.
| listItem          | [listItem][]  | Macht das **listItem** verfügbar, das Ziel dieser Aktivität war.

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a>Aktionen

Die Aktionen, die innerhalb einer Aktivität ausgeführt werden, sind detailliert in der **action**-Eigenschaft angegeben.
Nachstehend finden Sie die aktuell verfügbaren Aktionen.
Zukünftig werden möglicherweise neue Aktionen protokolliert, vergewissern Sie sich deshalb, ob Ihre App die Toleranz vonn **ItemActivity** ohne Aktionen unterstützt, die Ihre App versteht.

| Name der Aktion | Typ              | Beschreibung
|:------------|:------------------|:-------------------------------------------
| Kommentar     | [commentAction][] | Ein Kommentar wurde zu dem Element hinzugefügt.
| create      | [createAction][]  | Ein Element wurde erstellt.
| Löschen      | [deleteAction][]  | Ein Element wurde gelöscht.
| Bearbeiten        | [editAction][]    | Ein Element wurde bearbeitet.
| Erwähnung     | [mentionAction][] | Ein Benutzer wurde im Element erwähnt.
| verschieben        | [moveAction][]    | Ein Element wurde verschoben.
| rename      | [renameAction][]  | Ein Element wurde umbenannt.
| wiederherstellen     | [restoreAction][] | Ein Element wurde wiederhergestellt.
| freigeben       | [shareAction][]   | Ein Element wurde freigegeben.
| Version     | [versionAction][] | Ein Element wurde mit einer Versionsangabe versehen.

[accessAction]: accessaction.md
[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[location]: location.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a>Hinweise

**ItemActivity** ist zurzeit nur für SharePoint und OneDrive for Business verfügbar.

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity"
} -->
