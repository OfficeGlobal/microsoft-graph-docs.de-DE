---
title: Ressourcentyp outlookTaskGroup
description: 'Eine Gruppe von Ordnern (OutlookTaskFolder), die Outlook-Aufgaben (Auflistung von OutlookTask-Objekten) enthalten. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d1392e07f76d508fe30307294a54429a692f34e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923908"
---
# <a name="outlooktaskgroup-resource-type"></a>Ressourcentyp outlookTaskGroup

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine Gruppe von Ordnern ([OutlookTaskFolder](outlooktaskfolder.md)), die Outlook-Aufgaben (Auflistung von [OutlookTask](outlooktask.md) -Objekten) enthalten. 

In Outlook eine Aufgabe Standardgruppe vorhanden ist `My Tasks` das Umbenennen oder löschen können. Sie können jedoch zusätzliche Vorgangsgruppen erstellen. 


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von outlookTaskGroup](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |Rufen Sie die Eigenschaften und Beziehungen zwischen der angegebenen Gruppe der Outlook-Aufgabe.|
|[Erstellen von outlookTaskFolder](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Erstellen eines Outlook-Aufgabenordners.|
|[Liste taskFolders](../api/outlooktaskgroup-list-taskfolders.md) |[OutlookTaskFolder](outlooktaskfolder.md) -Auflistung| Rufen Sie eine Auflistung von Outlook Aufgabenordner.|
|[Update](../api/outlooktaskgroup-update.md) | [outlookTaskGroup](outlooktaskgroup.md)  |Aktualisieren Sie die schreibbaren Eigenschaften einer Outlook-Aufgabe-Gruppe. |
|[Delete](../api/outlooktaskgroup-delete.md) | Keine |Löschen der angegebenen Gruppe der Outlook-Aufgabe. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|changeKey|Zeichenfolge|Die Version der Aufgabengruppe.|
|groupKey|Edm.Guid|Der eindeutige GUID-Bezeichner für die Aufgabengruppe.|
|id|Zeichenfolge|Der eindeutige Zeichenfolgenbezeichner der Aufgabengruppe. Schreibgeschützt.|
|isDefaultGroup|Boolescher Wert|True, wenn die "Task Group" der Standardproxygruppe für die Aufgabe ist.|
|name|Zeichenfolge|Der Name der Aufgabengruppe.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|taskFolders|[OutlookTaskFolder](outlooktaskfolder.md) -Auflistung| Die Auflistung von Task-Ordner in der Aufgabengruppe. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}-->

```json
{
  "changeKey": "String",
  "groupKey": "Guid",
  "id": "String (identifier)",
  "isDefaultGroup": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
