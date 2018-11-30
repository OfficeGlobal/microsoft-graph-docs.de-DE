---
title: plannerTask-Ressourcentyp
description: Die **plannerTask**-Ressource stellt eine Planer-Aufgabe in Office 365 dar. Eine Planner-Aufgabe ist in einem Plan enthalten und kann einem Bucket in einem Plan zugewiesen werden. Jedes Aufgabenobjekt verfügt über ein details-Objekt, das weitere Informationen über die Aufgabe enthalten kann. Weitere Informationen zu Beziehungen zwischen Gruppe, Plan und Aufgabe finden Sie in der Übersicht.
ms.openlocfilehash: 75fedd01913d89121912b336420d4cc063165250
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019320"
---
# <a name="plannertask-resource-type"></a>plannerTask-Ressourcentyp

Die **plannerTask**-Ressource stellt eine Planer-Aufgabe in Office 365 dar. Eine Planner-Aufgabe ist in einem [Plan](plannerplan.md) enthalten und kann einem [Bucket](plannerbucket.md) in einem Plan zugewiesen werden. Jedes Aufgabenobjekt verfügt über ein [details](plannertaskdetails.md)-Objekt, das weitere Informationen über die Aufgabe enthalten kann. Weitere Informationen zu Beziehungen zwischen Gruppe, Plan und Aufgabe finden Sie in der [Übersicht](planner-overview.md).


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerTask abrufen](../api/plannertask-get.md) | [plannerTask](plannertask.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerTask**-Objekts.|
|[Aktualisieren](../api/plannertask-update.md) | [plannerTask](plannertask.md) |Dient zum Aktualisieren des **plannerTask**-Objekts. |
|[Löschen](../api/plannertask-delete.md) | Keine |Dient zum Löschen des **plannerTask**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|activeChecklistItemCount|Int32|Anzahl Prüflistenelemente, deren Wert auf „false“ festgelegt ist, was unvollständige Elemente darstellt.|
|appliedCategories|[plannerAppliedCategories](plannerappliedcategories.md)|Die Kategorien, auf die die Aufgabe angewendet wurde. Mögliche Werte finden Sie unter [angewendete Kategorien](plannerappliedcategories.md).|
|assigneePriority|String|Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.|
|assignments|[plannerAssignments](plannerassignments.md)|Der Satz von zugewiesenen Personen, denen die Aufgabe zugewiesen wurde.|
|bucketId|String|Bucket-ID, zu der die Aufgabe gehört. Der Bucket muss im Plan sein, die die Aufgabe ist. Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet. [Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst. |
|checklistItemCount|Int32|Anzahl der Prüflistenelemente, die für die Aufgabe vorhanden sind.|
|completedBy|[identitySet](identityset.md)|Die Identität des Benutzers, der die Aufgabe abgeschlossen hat.|
|completedDateTime|DateTimeOffset|Schreibgeschützt. Datum und Uhrzeit, zu dem bzw. der die `'percentComplete'` der Aufgabe auf `'100'` festgelegt ist. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|conversationThreadId|String|Thread-ID der Unterhaltung zur Aufgabe. Dies ist die ID des Unterhaltungsthreadobjekts, das in der Gruppe erstellt wurde.|
|createdBy|[identitySet](identityset.md)|Die Identität des Benutzers, der die Aufgabe erstellt hat.|
|createdDateTime|DateTimeOffset|Schreibgeschützt. Datum und Uhrzeit der Erstellung der Aufgabe. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|dueDateTime|DateTimeOffset|Datum und Uhrzeit der Fälligkeit der Aufgabe. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|hasDescription|Boolescher Wert|Schreibgeschützt. Der Wert ist `true`, wenn das Detailobjekt der Aufgabe eine nicht leere Beschreibung und aufweist, andernfalls `false`.|
|id|String|Schreibgeschützt. ID des Vorgangs. Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet. [Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.|
|orderHint|String|Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.|
|percentComplete|Int32|Abgeschlossener Prozentsatz der Aufgabe. Bei Festlegung auf `100` wird die Aufgabe als abgeschlossen betrachtet. |
|planId|String|Plan-ID, zu der die Aufgabe gehört.|
|previewType|plannerPreviewType|Hierdurch wird den Typ der Vorschau, die für den Vorgang wird angezeigt. Die möglichen Werte sind: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|referenceCount|Int32|Anzahl externer Bezüge, die für die Aufgabe vorhanden sind.|
|startDateTime|DateTimeOffset|Datum und Uhrzeit des Aufgabenbeginns. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|title|String|Titel der Aufgabe.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)| Schreibgeschützt. Lässt Nullwerte zu. Wird zum korrekten Rendern der Task Board-Ansicht bei Gruppierung nach assignedTo verwendet.|
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)| Schreibgeschützt. Lässt Nullwerte zu. Wird zum korrekten Rendern der Task Board-Ansicht bei Gruppierung nach Bucket verwendet.|
|Details|[plannerTaskDetails](plannertaskdetails.md)| Schreibgeschützt. Lässt Nullwerte zu. Weitere Details über die Aufgabe.|
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)| Schreibgeschützt. Lässt Nullwerte zu. Wird zum korrekten Rendern der Task Board-Ansicht bei Gruppierung nach Fortschritt verwendet.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTask"
}-->

```json
{
  "activeChecklistItemCount": 1024,
  "appliedCategories": {"@odata.type": "microsoft.graph.plannerAppliedCategories"},
  "assigneePriority": "String",
  "assignments": {"@odata.type": "microsoft.graph.plannerAssignments"},
  "bucketId": "String",
  "checklistItemCount": 1024,
  "completedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "completedDateTime": "String (timestamp)",
  "conversationThreadId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": true,
  "id": "String (identifier)",
  "orderHint": "String",
  "percentComplete": 1024,
  "planId": "String",
  "previewType": "string",
  "referenceCount": 1024,
  "startDateTime": "String (timestamp)",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
