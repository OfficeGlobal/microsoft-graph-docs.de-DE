---
title: AccessReview Reviewer entfernen
description: 'In Azure AD Access Feature überprüft, und Aktualisieren eines vorhandenen AccessReview-Objekts, um einen Benutzer als Bearbeiter zu entfernen.  Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden. Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden. '
localization_priority: Normal
ms.openlocfilehash: d33c1c2409b866a48d0684612f8c878e14dedb68
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866024"
---
# <a name="remove-accessreview-reviewer"></a>AccessReview Reviewer entfernen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [AccessReview](../resources/accessreview.md) -Objekts, um einen Benutzer als Bearbeiter zu entfernen.  Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden. Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden. 


## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | AccessReview.ReadWrite.All |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a>Anforderungsheader
| Name         | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| Authorization | string | Bearer \{token\}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Keine Anforderungstext sollte angegeben werden.


## <a name="response"></a>Antwort
Wenn erfolgreich, gibt diese Methode einen Antwortcode 200-Serie.

## <a name="example"></a>Beispiel

Dies ist ein Beispiel für eine einmalige (nicht wiederkehrenden) Access-Überprüfung zum Entfernen einer unnötige Reviewer aktualisieren.


##### <a name="request"></a>Anforderung
Geben Sie in der Anforderungs-URL die Id des AccessReview-Objekts, und klicken Sie dann die Id des Benutzerobjekts an.

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a>Antwort
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!-- {
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
