---
title: Ressourcentyp outlookTaskFolder
description: 'Ein Ordner mit Outlook-Aufgaben (Auflistung von OutlookTask-Objekten). '
ms.openlocfilehash: e3fb9d73dbd9458048749331d14f933d838d4243
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063653"
---
# <a name="outlooktaskfolder-resource-type"></a>Ressourcentyp outlookTaskFolder

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
|[Create single-value extended property](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |Erstellen Sie eine oder mehrere einwertig erweiterte Eigenschaften in einem neuen oder vorhandenen Outlook-Aufgabenordner.   |
|[Abrufen von Aufgabenordner mit erweiterten Eigenschaft einwertig](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Abrufen von Outlook-Aufgabenordner, die einen erweiterte Eigenschaft mithilfe von Single-Wert enthalten `$expand` oder `$filter`. |
|[Create multi-value extended property](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | Erstellen Sie eine oder mehrere erweiterte mehrwertige Eigenschaften in einem neuen oder vorhandenen Outlook-Aufgabenordner.  |
|[Abrufen von Aufgabenordner mit erweiterten Eigenschaft mit mehreren Werten](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Abrufen einer Outlook-Aufgabenordner, die mithilfe eine erweiterte Eigenschaft mit mehreren Werte enthält `$expand`. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|changeKey|String|Die Version des den Aufgabenordner.|
|id|String|Der Bezeichner des den Aufgabenordner, die im Postfach des Benutzers eindeutig. Schreibgeschützt.|
|isDefaultFolder|Boolesch|True, wenn der Ordner der Standardordner für die Aufgabe ist.|
|name|String|Der Name des Aufgabenordners.|
|parentGroupKey|Guid|Der eindeutige GUID-Bezeichner für die übergeordnete Gruppe des vorgangsordners.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung|Die Auflistung der Mehrfachwert erweiterte Eigenschaften für den Aufgabenordner definiert. Schreibgeschützt. Lässt Nullwerte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung|Die Auflistung der einwertig erweiterte Eigenschaften für den Aufgabenordner definiert. Schreibgeschützt. Lässt Nullwerte zu.|
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->