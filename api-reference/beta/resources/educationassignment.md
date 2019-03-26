---
title: educationAssignment-Ressourcentyp
description: Die **educationAssignment** -Ressource stellt eine Aufgabe oder eine Arbeitseinheit dar, die einem Schüler oder Teammitglied in einer Klasse als Teil ihrer Studie zugeordnet ist. Nur Lehrer oder Teambesitzer können Zuordnungen erstellen. Zuordnungen enthalten Handzettel und Aufgaben, an denen der Kursteilnehmer arbeiten möchte. Jede Schüler Zuweisung hat eine zugeordnete Übermittlung, die alle arbeiten enthält, die Ihr Lehrer zum Einschalten beantragt hat. Ein Lehrer kann Partituren und Feedback zu der vom Schüler eingestellten Einsendung hinzufügen.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 03612cd65dbefac4e31f1a4d06085ba635fe1eab
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30800005"
---
# <a name="educationassignment-resource-type"></a>educationAssignment-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **educationAssignment** -Ressource stellt eine Aufgabe oder eine Arbeitseinheit dar, die einem Schüler oder Teammitglied in einer Klasse als Teil ihrer Studie zugeordnet ist. Nur Lehrer oder Teambesitzer können Zuordnungen erstellen. Zuordnungen enthalten Handzettel und Aufgaben, an denen der Kursteilnehmer arbeiten möchte. Jede Schüler Zuweisung hat eine zugeordnete [Übermittlung](educationsubmissionresource.md) , die alle arbeiten enthält, die Ihr Lehrer zum Einschalten beantragt hat. Ein Lehrer kann Partituren und Feedback zu der vom Schüler eingestellten Einsendung hinzufügen.

Wenn eine Zuordnung erstellt wird, befindet Sie sich im Entwurfszustand. Die Teilnehmer können die Zuordnung nicht sehen, und die Übermittlungen werden nicht erstellt. Sie können den Status einer Zuordnung mithilfe der Aktion [veröffentlichen](../api/educationassignment-publish.md) ändern. Sie können keine PATCH-Anforderung verwenden, um den Zuordnungsstatus zu ändern.

Die Zuweisungs-APIs werden im Klassennamespace verfügbar gemacht.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Zuweisung abrufen](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |Liest die Eigenschaften und Beziehungen eines **educationAssignment** -Objekts.|
|[Zugeordnete Ressource erstellen](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| Erstellen Sie eine neue **educationAssignmentResource** durch veröffentlichen in der Resources-Auflistung.|
|[Ressourcen aufListen](../api/educationassignment-list-resources.md) |[educationAssignmentResource](educationassignmentresource.md) -Sammlung| Rufen Sie eine **educationAssignmentResource** -Objektsammlung ab.|
|[AufListen von Übermittlungen](../api/educationassignment-list-submissions.md) |[educationSubmission](educationsubmission.md) -Sammlung| Rufen Sie eine **educationSubmission** -Objektsammlung ab.|
|[Kategorien auflisten](../api/educationassignment-list-categories.md) |[educationCategory](educationcategory.md) -Sammlung| Rufen Sie eine **educationCategory** -Objektsammlung ab.|
|[Kategorien hinzufügen](../api/educationassignment-add-categories.md) |[educationCategory](educationcategory.md) | Weisen Sie dieser Zuordnung ein **educationCategory** zu, das der Klasse angehört.|
|[Kategorie entfernen](../api/educationassignment-remove-category.md) |Keines| Entfernen Sie aus dieser Zuordnung ein **educationCategory** , das zur Klasse gehört.|
|[Update](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |Aktualisieren eines **educationAssignment** -Objekts. |
|[Löschen](../api/educationassignment-delete.md) | Keine |Löscht ein **educationAssignment** -Objekt. |
|[Publish](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|Ändern Sie den Status eines **educationAssignment** -Objekts von Entwurf in veröffentlicht.|
|[URL für Ressourcenordner abrufen](../api/educationassignment-getresourcesfolderurl.md)| Zeichenfolge| Der OneDrive-Ordner, in dem dateibasierte Ressourcen als Teil einer Zuordnungs Ressource gespeichert werden sollen. Dateien müssen sich in diesem Ordner befinden, damit Sie als Ressource hinzugefügt werden können.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt.|
|allowLateSubmissions|Boolesch| Gibt an, ob Schüler nach dem Fälligkeitsdatum übermitteln können. Wenn diese Eigenschaft nicht während der Erstellung angegeben wird, wird standardmäßig true festgelegt. |
|allowStudentsToAddResourcesToSubmission|Boolesch| Gibt an, ob Schüler eigene Ressourcen zu einer Übermittlung hinzufügen können oder ob Sie nur vom Lehrer hinzugefügte Ressourcen ändern können. |
|assignDateTime|DateTimeOffset|Das Datum, an dem die Zuordnung aktiv werden soll.  Wenn in der Zukunft die Zuordnung bis zu diesem Datum nicht angezeigt wird.  Der **timestamp** -Typ stellt Datums-und Uhrzeitinformationen unter Verwendung des ISO 8601-Formats dar und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| Die Benutzer oder die ganze Klasse sollten ein Submission-Objekt empfangen, nachdem die Zuordnung veröffentlicht wurde. |
|assignedDateTime|DateTimeOffset|Der Zeitpunkt, zu dem die Zuweisung für Schüler veröffentlicht wurde und die Zuordnung auf der Zeitachse der Kursteilnehmer angezeigt wird.  Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|classId|String| Klasse, zu der diese Zuordnung gehört. |
|createdBy|[identitySet](identityset.md)| Wer hat die Zuordnung erstellt? |
|createdDateTime|DateTimeOffset|Zeitpunkt, zu dem die Zuordnung erstellt wurde.  Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|displayName|Zeichenfolge|Der Name der Zuordnung.|
|dueDateTime|DateTimeOffset|Das Datum, an dem die Zuweisung der Teilnehmer fällig ist.  Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Benotung|[educationAssignmentGradeType](educationassignmentgradetype.md)|Wie die Zuweisung benotet wird. |
|Anweisungen|[itemBody](itembody.md)| Anweisungen für die Zuordnung.  Dieser zusammen mit dem Anzeigenamen teilen Sie dem Kursteilnehmer mit, was zu tun ist. |
|lastModifiedBy|[identitySet](identityset.md)| Die die Zuordnung zuletzt geändert hat. |
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt, zu dem die Zuordnung zuletzt geändert wurde.  Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|status|string| Status der **Zuordnung**.  Sie können diesen Wert nicht PATCHen.  Mögliche Werte sind: `draft`, `published` und `assigned`.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Ressourcen|[educationAssignmentResource](educationassignmentresource.md) -Sammlung| Lernobjekte, die dieser Zuordnung zugeordnet sind.  Nur Lehrer können diese Liste ändern. Lässt Nullwerte zu.|
|Einreichungen|[educationSubmission](educationsubmission.md) -Sammlung| Sobald veröffentlicht, gibt es ein Submission-Objekt für jeden Schüler, der Ihre Arbeit und Besoldungsgruppe darstellt.  Schreibgeschützt. Lässt Nullwerte zu.|
|categories|[educationCategory](educationcategory.md) -Sammlung| Wenn diese Option festgelegt ist, können Benutzer problemlos Zuordnungen eines bestimmten Typs finden.  Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "String (timestamp)",
  "classId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "dueDateTime": "String (timestamp)",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "instructions": {"@odata.type": "microsoft.graph.itemBody"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "status": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
