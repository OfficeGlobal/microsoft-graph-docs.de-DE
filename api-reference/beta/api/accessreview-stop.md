---
title: AccessReview beenden
description: In Azure AD Access Feature überprüft, und beenden Sie eine derzeit aktive AccessReview.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.  (Um zu verhindern, dass sich wiederholenden Access Wiederholung zukünftige Instanzen starten, aktualisieren Sie, um die geplante Enddatum ändern).  Überprüfen Sie nach dem Zugriff wird beendet, Bearbeiter können nicht mehr liefern Input und die Zugriff überprüfen Entscheidungen angewendet werden können.
localization_priority: Normal
ms.openlocfilehash: 57c0473b58b8ca4bbbb4e9f182b7da4582af4c38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860116"
---
# <a name="stop-accessreview"></a>AccessReview beenden

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Beenden Sie eine derzeit aktive [AccessReview](../resources/accessreview.md)in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.  (Sie wiederkehrende Access Wiederholung verhindern, dass zukünftige Instanzen, so ändern Sie das Enddatum des geplanten [Aktualisieren](accessreview-update.md) ).  Überprüfen Sie nach dem Zugriff wird beendet, Bearbeiter können nicht mehr liefern Input und die Zugriff überprüfen Entscheidungen angewendet werden können.
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
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a>Anforderungsheader
| Name         | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| Authorization | string | Bearer \{token\}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.


## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/stop()
```
##### <a name="response"></a>Antwort
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
