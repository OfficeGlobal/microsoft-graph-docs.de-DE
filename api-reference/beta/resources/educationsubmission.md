---
title: Ressourcentyp educationSubmission
description: Übermittlungen gehören eine Zuordnung. Eine Übermittlung stellt die Ressourcen, die eine einzelne (oder Gruppe) aktivieren im für eine Zuordnung und Note/Feedback zurückgegeben wird.
author: dipakboyed
ms.openlocfilehash: 5535aef4db988e0f4c4417128b5b53bbed884cc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328021"
---
# <a name="educationsubmission-resource-type"></a>Ressourcentyp educationSubmission

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Übermittlungen gehören eine Zuordnung. Eine Übermittlung stellt die Ressourcen, die eine einzelne (oder Gruppe) aktivieren im für eine Zuordnung und Note/Feedback zurückgegeben wird.
Übermittlungen werden automatisch erstellt, wenn eine Zuordnung veröffentlicht wird. Die Übermittlung besitzt zwei Listen mit Ressourcen. Ressourcen darstellen, die Benutzer/Gruppen Bereich arbeiten, während die gesendeten Ressourcen die Ressourcen darstellen, die aktiv Kursteilnehmer aktiviert wurde.  

>**Hinweis:** Der Status ist schreibgeschützt, und das Objekt wird durch den Workflow über Aktionen verschoben. 

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von educationSubmission](../api/educationsubmission-get.md) | [educationSubmission](educationsubmission.md) |Lesen Sie Eigenschaften und die Beziehungen eines **EducationSubmission** -Objekts.|
|[List-Ressourcen](../api/educationsubmission-list-resources.md) |[EducationSubmissionResource](educationsubmissionresource.md) -Auflistung| Rufen Sie eine Auflistung der **EducationSubmissionResource** -Objekts.|
|[Liste submittedResources](../api/educationsubmission-list-submittedresources.md) |[EducationSubmissionResource](educationsubmissionresource.md) -Auflistung| Rufen Sie eine Auflistung der **EducationSubmissionResource** -Objekts.|
|[Update](../api/educationsubmission-update.md) | [educationSubmission](educationsubmission.md) |Aktualisieren eines **EducationSubmission** -Objekts. |
|[Return](../api/educationsubmission-return.md)|[educationSubmission](educationsubmission.md)|Lehrer wird Return verwendet, um anzugeben, dass das Klasse/Feedback der Student angezeigt werden können.|
|[Senden](../api/educationsubmission-submit.md)|[educationSubmission](educationsubmission.md)|Einen Schüler verwendet übermitteln, um die Zuordnung zu aktivieren. Dadurch wird die Ressourcen in den Ordner **SubmittedResources** für Benotung kopiert und aktualisiert den Status.|
|[Unsubmit](../api/educationsubmission-unsubmit.md)|[educationSubmission](educationsubmission.md)|Ein Schüler verwendet die Unsubmit zum Verschieben des Status der Übermittlung von gesendete Back zu arbeiten. Dadurch wird die Ressourcen in den Ordner **WorkingResources** für Benotung kopiert und aktualisiert den Status.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Feedback|[educationFeedback](educationfeedback.md)|Enthält die Feedback-Eigenschaft, die des Lehrers Hinweise wieder für Studenten gespeichert.|
|grade|[educationAssignmentGrade](educationassignmentgrade.md)|Enthält die Klasse Informationen, die diese Übermittlung Lehrer zuweist.|
|id|String| Schreibgeschützt.|
|Empfänger|[educationSubmissionRecipient](educationsubmissionrecipient.md)|Die diese Übermittlung zugewiesen ist.|
|releasedBy|[identitySet](identityset.md)|Benutzer, der den Status dieser Übermittlung freigegeben verschoben.|
|releasedDateTime|DateTimeOffset|Bei die Übermittlung veröffentlicht wurde Zeitpunkt. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|returnedBy|[identitySet](identityset.md)|Benutzer, der den Status dieser Übermittlung zurückgegeben verschoben.|
|returnedDateTime|DateTimeOffset|Bei die Übermittlung zurückgegeben wurde Zeitpunkt. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|resourcesFolderUrl|String|Ordner, in denen alle Ressourcen für die Versendung gespeichert werden müssen.|
|status|string| Schreibgeschützt. Mögliche Werte: `working`, `submitted`, `released`, `returned`.|
|submittedBy|[identitySet](identityset.md)|Benutzer, die die Ressource in den gesendeten Zustand verschoben.|
|submittedDateTime|DateTimeOffset|Bei die Übermittlung in den gesendeten Zustand verschoben wurde Zeitpunkt. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|unsubmittedBy|[identitySet](identityset.md)|Benutzer, der die Ressource verschoben von übermittelt, in den Arbeitszustand.|
|unsubmittedDateTime|DateTimeOffset|Bei die Übermittlung von verschoben wurde übermittelt, in den Arbeitszustand Zeitpunkt. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|resources|[EducationSubmissionResource](educationsubmissionresource.md) -Auflistung| Lässt Nullwerte zu.|
|submittedResources|[EducationSubmissionResource](educationsubmissionresource.md) -Auflistung| Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "grade": {"@odata.type": "microsoft.graph.educationAssignmentGrade"},
  "id": "String (identifier)",
  "recipient": {"@odata.type": "microsoft.graph.educationSubmissionRecipient"},
  "returnedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "returnedDateTime": "String (timestamp)",
  "resourcesFolderUrl": "String",
  "status": "string",
  "submittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "submittedDateTime": "String (timestamp)",
  "unsubmittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "unsubmittedDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->