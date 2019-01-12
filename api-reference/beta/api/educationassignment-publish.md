---
title: 'EducationAssignment: Veröffentlichen'
description: Diese Aktion, die den Status einer Zuordnung aus der ursprünglichen Entwurfsstatus in der veröffentlichten Status geändert wird. Nur in der Klasse Lehrer kann diese aufrufen. Eine Zuordnung im Status "Entwurf" ist, Studenten die Zuordnung werden nicht angezeigt, noch werden die Übermittlung Objekte vorhanden sein. Wenn Sie diese API aufrufen, Übermittlung Objekte erstellt werden, und die Zuordnung in der Student-Liste angezeigt wird.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: c7cdaebb91490270cc0a8f205b41a89b662a7a13
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926701"
---
# <a name="educationassignment-publish"></a>EducationAssignment: Veröffentlichen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Diese Aktion, die den Status einer Zuordnung aus der ursprünglichen Entwurfsstatus in der veröffentlichten Status geändert wird. Nur in der Klasse Lehrer kann diese aufrufen. Eine Zuordnung im Status "Entwurf" ist, Studenten die Zuordnung werden nicht angezeigt, noch werden die Übermittlung Objekte vorhanden sein. Wenn Sie diese API aufrufen, Übermittlung Objekte erstellt werden, und die Zuordnung in der Student-Liste angezeigt wird.

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
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a>Anforderungsheader
| Header       | Wert |
|:---------------|:--------|
| Authorization  | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.
##### <a name="request"></a>Anforderung
Es folgt ein Beispiel für eine Anforderung.
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a>Antwort
Es folgt ein Beispiel für eine Antwort. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
