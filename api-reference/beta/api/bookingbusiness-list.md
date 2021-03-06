---
title: Liste bookingBusinesses
description: Rufen Sie eine Auflistung von Bookingbusiness-Objekten, die erstellt wurde, für den Mandanten.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 8018b8ac7f9d2e5f74e4233dbc36c2a6faa2d9a8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523155"
---
# <a name="list-bookingbusinesses"></a>Liste bookingBusinesses

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rufen Sie eine Auflistung von [Bookingbusiness](../resources/bookingbusiness.md) -Objekten, die erstellt wurde, für den Mandanten.

Dieser Vorgang gibt nur die **Id** und **DisplayName** jedes Buchungen Unternehmens in der Auflistung zurück. Unter Leistungsgesichtspunkten gibt es keine anderen Eigenschaften zurück. Sie können die anderen Eigenschaften eines Unternehmens Buchungen abrufen, indem dessen **Id** angeben, in einem Vorgang [erhalten möchten](bookingbusiness-get.md) .

Sie können auch für Unternehmen Buchungen Abfragen, durch Angeben einer Zeichenfolge in einer `query` Parameter untergeordnete Zeichenfolgen Übereinstimmung zwischen dem Unternehmen eines Mandanten liegen. Unten finden Sie ein [Beispiel](#request-2).


## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt   |
|Anwendung | Nicht unterstützt  |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

Diese Methode unterstützt die `query` -Parameter der akzeptiert einen String-Wert. Dieser Parameter beschränkt das Abrufen der Ergebnisse an Unternehmen, die der angegebenen Zeichenfolge entsprechen. Sehen Sie ein [Beispiel](#request-2) unten ein.


## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [BookingBusiness](../resources/bookingbusiness.md) .
## <a name="example"></a>Beispiel
##### <a name="request-1"></a>Anforderung 1
Im folgenden Beispiel wird die Buchungen Unternehmen in einem Mandanten.
<!-- {
  "blockType": "request",
  "name": "get_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
```
##### <a name="response-1"></a>Antwort 1
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"Contosolunchdelivery@M365B489948.onmicrosoft.com",
            "displayName":"Contoso lunch delivery",
        },
        {
            "id":"Fabrikam@M365B489948.onmicrosoft.com",
            "displayName":"Fabrikam",
        }
    ]
}
```


##### <a name="request-2"></a>Anforderung 2
Das folgende Beispiel zeigt, wie Sie mit der `query` Parameter zum Abrufen von mindestens einen übereinstimmender Buchungen Unternehmen in den Mandanten.
<!-- {
  "blockType": "request",
  "name": "query_bookingbusinesses"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Adventure
```
##### <a name="response-2"></a>Antwort 2
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"AdventureWorksCycles@M365B960066.onmicrosoft.com",
            "displayName":"Adventure Works Cycles",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
