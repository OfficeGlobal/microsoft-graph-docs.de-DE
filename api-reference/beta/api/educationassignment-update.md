---
title: Educationassignment aktualisieren
description: Aktualisieren Sie das Assignment-Objekt. Nur Lehrer in der Klasse ist dies möglich. Beachten Sie, dass eine Anforderung PATCH zum Ändern des Status einer Zuordnung verwendet werden können. Verwenden Sie die Veröffentlichungsaktion zum Ändern des Zuordnungsstatus.
ms.openlocfilehash: 8b23b7ac4b971856ed7a96b4991fca2e5220d069
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060894"
---
# <a name="update-educationassignment"></a>Educationassignment aktualisieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Aktualisieren Sie das Assignment-Objekt. Nur Lehrer in der Klasse ist dies möglich. Beachten Sie, dass eine Anforderung PATCH zum Ändern des Status einer Zuordnung verwendet werden können. Verwenden Sie die Aktion [Veröffentlichen](../api/educationassignment-publish.md) , um den Status einer Aufgabe ändern.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  EduAssignments.ReadWriteBasic EduAssignments.ReadWrite  |
|Delegiert (persönliches Microsoft-Konto) |  Nicht unterstützt  |
|Anwendung | Nicht unterstützt | 

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowLateSubmissions|Boolesch| Gibt an, ob nach dem Fälligkeitsdatum Übermittlungen gesendet werden können.|
|allowStudentsToAddResourcesToSubmission|Boolesch| Gibt an, ob eine Student Ressourcen zu einer Übermittlung hinzufügen kann. Angegeben, ob die Ressourcenliste Zuordnung der einzige Elemente auf der Übermittlung stammt. |
|assignDateTime|DateTimeOffset| Datum, an dem die Zuordnung für Studenten veröffentlicht werden soll. |
|assignTo|educationAssignmentRecipient| Teilnehmer, die die Zuordnung zu erhalten.|
|displayName|String| Name der Zuordnung. |
|dueDateTime|DateTimeOffset| Datum Aufgabe ist fällig. |
|Benotung|educationAssignmentGradeType| Wie wird die Zuordnung eingestuft.|
|Anleitung|itemBody| Anleitung für die Kursteilnehmer zusammen mit der Zuordnung angegeben. |

## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [EducationAssignment](../resources/educationassignment.md) -Objekts in der Antworttext.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002
Content-type: application/json
Content-length: 279

{
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. 

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "classId": "11021",
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->