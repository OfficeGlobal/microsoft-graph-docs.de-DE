---
title: Ressourcentyp outlookTaskFolder
description: 'Ein Ordner mit Outlook-Aufgaben (Auflistung von OutlookTask-Objekten). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eb61936b9ede67d35127db07c92ba8b7517fe623
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515300"
---
# <a name="outlooktaskfolder-resource-type"></a>Ressourcentyp outlookTaskFolder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Ordner mit Outlook-Aufgaben (Auflistung von [OutlookTask](outlooktask.md) -Objekten). 

In Outlook, der Standardgruppe Aufgabe `My Tasks`, enthält einen Standardordner Aufgabe `Tasks`, für das Postfach des Benutzers. Sie umbenennen oder löschen Sie diese Aufgabe Standardgruppe und der Ordner ist nicht möglich, aber Sie können zusätzliche Vorgangsgruppen und Aufgabenordner erstellen.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von outlookTaskFolder](../api/outlooktaskfolder-get.md) | [outlookTaskFolder](outlooktaskfolder.md) |Rufen Sie die Eigenschaften und Beziehungen zwischen den angegebenen Outlook-Aufgabenordner.|
|[Erstellen von outlookTask](../api/outlooktaskfolder-post-tasks.md) |[outlookTask](outlooktask.md)| Erstellen Sie eine Outlook-Aufgabe im angegebenen Ordner.|
|[Aufgaben auflisten](../api/outlooktaskfolder-list-tasks.md) |[OutlookTask](outlooktask.md) -Auflistung| Rufen Sie die Outlook-Aufgaben im angegebenen Ordner.|
|[Update](../api/outlooktaskfolder-update.md) | [outlookTaskFolder](outlooktaskfolder.md)   |Aktualisieren Sie die schreibbaren Eigenschaften des Ordners eine Outlook-Aufgabe. |
|[Delete](../api/outlooktaskfolder-delete.md) | Keine |Den angegebenen Outlook den Ordner zu löschen.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |Erstellen Sie eine oder mehrere einwertig erweiterte Eigenschaften in einem neuen oder vorhandenen Outlook-Aufgabenordner.   |
|[Abrufen von Aufgabenordner mit erweiterten Eigenschaft einwertig](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Abrufen von Outlook-Aufgabenordner, die einen erweiterte Eigenschaft mithilfe von Single-Wert enthalten `$expand` oder `$filter`. |
|[Mehrwertige erweiterte Eigenschaft erstellen](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | Erstellen Sie eine oder mehrere erweiterte mehrwertige Eigenschaften in einem neuen oder vorhandenen Outlook-Aufgabenordner.  |
|[Abrufen von Aufgabenordner mit erweiterten Eigenschaft mit mehreren Werten](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Abrufen einer Outlook-Aufgabenordner, die mithilfe eine erweiterte Eigenschaft mit mehreren Werte enthält `$expand`. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|changeKey|String|Die Version des den Aufgabenordner.|
|id|Zeichenfolge|Der Bezeichner des den Aufgabenordner, die im Postfach des Benutzers eindeutig. Schreibgeschützt.|
|isDefaultFolder|Boolescher Wert|True, wenn der Ordner der Standardordner für die Aufgabe ist.|
|name|Zeichenfolge|Der Name des Aufgabenordners.|
|parentGroupKey|Guid|Der eindeutige GUID-Bezeichner für die übergeordnete Gruppe des vorgangsordners.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung|Die Auflistung der Mehrfachwert erweiterte Eigenschaften für den Aufgabenordner definiert. Schreibgeschützt. Nullwerte zulassend.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung|Die Auflistung der einwertig erweiterte Eigenschaften für den Aufgabenordner definiert. Schreibgeschützt. Nullwerte zulassend.|
|tasks|[OutlookTask](outlooktask.md) -Auflistung|Die Aufgaben in diesem Aufgabenordner. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}-->

```json
{
  "changeKey": "String",
  "id": "String (identifier)",
  "isDefaultFolder": true,
  "name": "String",
  "parentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlooktaskfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
