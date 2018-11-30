---
title: AccessReview Bearbeiter hinzufügen
description: 'In Azure AD Access Feature überprüft, und Aktualisieren eines vorhandenen AccessReview-Objekts, um einen anderen Benutzer als ein Prüfer hinzuzufügen.  Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden. Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden. '
ms.openlocfilehash: ac7722d1bea30659db6f6defe26c0a08ecd67caf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060645"
---
# <a name="add-accessreview-reviewer"></a>AccessReview Bearbeiter hinzufügen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [AccessReview](../resources/accessreview.md) -Objekts, um einen anderen Benutzer als ein Prüfer hinzuzufügen.  Dieser Vorgang ist nur zulässig für eine Access-Überprüfung, die noch nicht abgeschlossen ist, und nur für eine Access-Überprüfung, wobei die Bearbeiter explizit angegeben werden. Dieser Vorgang ist nicht zulässig für eine Access-Überprüfung in der Benutzer ihre eigenen Access überprüfen und nicht für die direkte Verwendung für eine Access-Überprüfung in der Gruppenbesitzer als Bearbeiter zugewiesen werden. 


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
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a>Anforderungsheader
| Name         | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| Authorization | string | Bearer \{token\}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung der ID des Benutzers ein, die einem Bearbeiter werden.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die beim Aktualisieren von einer AccessReview bereitgestellt werden können.

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | Die Benutzer-ID.  |


## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201, Created` Antwortcode.

## <a name="example"></a>Beispiel

Dies ist ein Beispiel für eine einmalige (nicht wiederkehrenden) Access Überprüfung mit einer weiteren Person aktualisiert.

##### <a name="request"></a>Anforderung
Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Id des User-Objekts.

<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
Content-type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```

##### <a name="response"></a>Antwort
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!-- {
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
