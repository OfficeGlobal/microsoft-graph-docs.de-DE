---
title: Ressourcentyp educationAssignment
description: Die Ressource **EducationAssignment** stellt einen Vorgang oder eine Arbeitsschritt Mitglied Student oder ein Team in einer Klasse als Teil ihrer Studie zugewiesen. Nur Lehrer oder Team Besitzer können Zuordnungen erstellen. Zuordnungen enthalten, Handzettel und Aufgaben, die die Lehrer den Teilnehmern an arbeiten möchte. Jeder Student Zuordnung hat offenem zugeordnet, die keine Arbeit enthält, die ihre Lehrer aufgefordert werden, die deaktiviert werden. Lehrer kann Bewertungen und Feedback der Übermittlung von den Teilnehmern Unternehmensadministrator hinzufügen.
ms.openlocfilehash: c95197edd5f1ed821ca83171d74f0beee300eb1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061810"
---
# <a name="educationassignment-resource-type"></a>Ressourcentyp educationAssignment

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Ressource **EducationAssignment** stellt einen Vorgang oder eine Arbeitsschritt Mitglied Student oder ein Team in einer Klasse als Teil ihrer Studie zugewiesen. Nur Lehrer oder Team Besitzer können Zuordnungen erstellen. Zuordnungen enthalten, Handzettel und Aufgaben, die die Lehrer den Teilnehmern an arbeiten möchte. Jeder Student Zuordnung hat eine zugeordnete [Übermittlung](educationsubmissionresource.md) , die keine Arbeit enthält, die ihre Lehrer aufgefordert werden, die deaktiviert werden. Lehrer kann Bewertungen und Feedback der Übermittlung von den Teilnehmern Unternehmensadministrator hinzufügen.

Wenn eine Zuordnung erstellt wird, ist es im Entwurfszustand. Studenten nicht die Zuordnung angezeigt und Übermittlungen nicht erstellt werden. Sie können den Status einer Zuordnung ändern, mit der Aktion [Veröffentlichen](../api/educationassignment-publish.md) . Sie können keine Anforderung PATCH verwenden, um den Status einer Aufgabe zu ändern.

Die Zuordnung APIs werden in den Klassennamespace verfügbar gemacht.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen der Zuordnung](../api/educationassignment-get.md) | [educationAssignment](educationassignment.md) |Lesen Sie Eigenschaften und die Beziehungen eines **EducationAssignment** -Objekts.|
|[Erstellen der Zuordnung Ressource](../api/educationassignment-post-resources.md) |[educationAssignmentResource](educationassignmentresource.md)| Erstellen Sie eine neue **EducationAssignmentResource** , indem Sie das Veröffentlichen in der Resources-Auflistung.|
|[List-Ressourcen](../api/educationassignment-list-resources.md) |[EducationAssignmentResource](educationassignmentresource.md) -Auflistung| Rufen Sie eine Auflistung der **EducationAssignmentResource** -Objekts.|
|[Liste Übermittlungen](../api/educationassignment-list-submissions.md) |[EducationSubmission](educationsubmission.md) -Auflistung| Rufen Sie eine Auflistung der **EducationSubmission** -Objekts.|
|[Update](../api/educationassignment-update.md) | [educationAssignment](educationassignment.md) |Aktualisieren eines **EducationAssignment** -Objekts. |
|[Delete](../api/educationassignment-delete.md) | Keine |Löschen eines **EducationAssignment** -Objekts. |
|[Publish](../api/educationassignment-publish.md)|[educationAssignment](educationassignment.md)|Ändern Sie den Status eines Objekts **EducationAssignment** von Entwurf, veröffentlicht.|
|[Abrufen der Ressource Ordner-URL](../api/educationassignment-getresourcesfolderurl.md)| string| Der OneDrive-Ordner in den Ressourcen dateibasierten platziert werden soll, um eine Zuordnung Ressource angehören. In diesem Ordner als Ressource hinzugefügt werden müssen sich Dateien befinden.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt.|
|allowLateSubmissions|Boolesch| Bestimmt, ob nach dem Fälligkeitsdatum Studenten übermitteln können. Wenn diese Eigenschaft nicht bei der Erstellung angegeben wird, wird standardmäßig auf "true". |
|allowStudentsToAddResourcesToSubmission|Boolesch| Gibt an, ob die eigene Ressourcen einer Übermittlung hinzugefügt werden können oder wenn sie nur Ressourcen hinzugefügt werden die Lehrer ändern können. |
|assignDateTime|DateTimeOffset|Das Datum, wenn die Zuordnung aktiv werden sollen.  Wenn in der Zukunft wird die Zuordnung nicht zum Schüler bis zum aktuellen Datum angezeigt.  Der **Zeitstempel** Typ stellt Informationen zum Datum und Uhrzeit mit ISO 8601-Format dar und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|assignTo|[educationAssignmentRecipient](educationassignmentrecipient.md)| Welche Benutzer oder die gesamte Klasse sollte ein Objekt zum Absenden erhalten, nachdem die Zuordnung veröffentlicht wird. |
|assignedDateTime|DateTimeOffset|Auf der Zeitachse Studenten wird der Zeitpunkt, den die Zuordnung in Studenten und die Zuordnung veröffentlicht wurde.  Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|classId|String| Klasse, die diese Zuordnung gehört. |
|createdBy|[identitySet](identityset.md)| Die die Zuordnung erstellt. |
|createdDateTime|DateTimeOffset|Zeitpunkt der Erstellung die Zuordnung.  Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|displayName|String|Name der Zuordnung.|
|dueDateTime|DateTimeOffset|Datum die Studenten-Zuordnung fällig ist.  Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Benotung|[educationAssignmentGradeType](educationassignmentgradetype.md)|Wie wird die Zuordnung eingestuft. |
|Anleitung|[itemBody](itembody.md)| Anleitung für die Zuordnung.  Dies zusammen mit dem Anzeigenamen lassen Sie den Kursteilnehmer Aktionen. |
|lastModifiedBy|[identitySet](identityset.md)| Die die Zuordnung der letzten Änderung. |
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt der letzten die Zuordnung Änderung.  Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|status|string| Status der **Zuordnung**.  Sie können nicht PATCH dieser Wert.  Mögliche Werte sind: `draft`, `published` und `assigned`.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|resources|[EducationAssignmentResource](educationassignmentresource.md) -Auflistung| Learning-Objekte, die diese Zuordnung zugeordnet sind.  Nur Lehrer können diese Liste ändern. Lässt Nullwerte zu.|
|Übermittlungen|[EducationSubmission](educationsubmission.md) -Auflistung| Nachdem veröffentlicht, ist es ein Übermittlung-Objekt für jeden Kursteilnehmer, ihre Arbeit und Note darstellt.  Schreibgeschützt. Lässt Nullwerte zu.|

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
