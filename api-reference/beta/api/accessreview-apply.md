---
title: Anwenden von accessReview
description: 'In Azure AD zugreifen auf Berichte-Funktion, anwenden Sie die Entscheidungen von einer abgeschlossenen AccessReview.  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9612f3bcb8a032ee32cd7b058d3f21950c9b120f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512213"
---
# <a name="apply-accessreview"></a>Anwenden von accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gelten Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature die Entscheidungen von einer abgeschlossenen [AccessReview](../resources/accessreview.md).  Das Zielobjekt kann entweder eine einmalige Access Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung sein.  


Nach Abschluss eine Access-Überprüfung entweder, da es das Enddatum erreicht oder ein Administrator manuell angehalten, und automatisch zugewiesenes wurde nicht konfiguriert für die Überprüfung können Sie aufrufen, übernehmen, um die Änderungen zu übernehmen. Bis übernehmen auftritt, erscheinen die Entscheidungen Zugriffsrechte entfernen nicht für die Ressource Quelle die Benutzer ihrer Gruppenmitgliedschaften für die Instanz beibehalten werden. Durch Aufrufen von anwendbar sind, wird das Ergebnis der Überprüfung durch Aktualisieren der Gruppe oder einer Anwendung implementiert. Wenn Sie den Zugriff eines Benutzers bei der Überprüfung verweigert wurde, wenn ein Administrator diese API aufruft, entfernt Azure AD ihre Aufgaben Mitgliedschaft oder der Anwendung an. 

Nach eine Access-Überprüfung abgeschlossen ist, und automatisch zugewiesenes wurde so konfiguriert, und klicken Sie dann der Status der Überprüfung von abgeschlossen durch intermediate Zustände geändert und schließlich Applied Status geändert wird. Sie sollten verweigerte Benutzer sehen erwarten, wenn vorhanden, wird von der Ressource entfernt Mitgliedschaft oder app-Zuordnung in ein paar Minuten gruppieren.

Eine konfigurierte automatische Überprüfung anwenden, oder übernehmen auswählen keinen Effekt auf eine Gruppe, die in einem lokalen Verzeichnis stammt oder eine dynamische Gruppe. Wenn Sie eine Gruppe ändern, die lokalen stammt möchten, laden Sie die Ergebnisse und gelten Sie diese Änderungen für die Darstellung der Gruppe in dieses Verzeichnis.


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
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a>Anforderungsheader
| Name         | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| Authorization | string | Bearertoken Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.


## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="see-also"></a>Siehe auch

- [Wie Sie für die Durchführung eine Access-Überprüfung](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
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
<!--
{
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
