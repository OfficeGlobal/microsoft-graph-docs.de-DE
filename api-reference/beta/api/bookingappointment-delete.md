---
title: BookingAppointment löschen
description: Löschen einer BookingAppointment in der angegebenen Bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a8abe1961be7e3caf36c9d690497347f42c83fde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513718"
---
# <a name="delete-bookingappointment"></a>BookingAppointment löschen

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Löschen einer [BookingAppointment](../resources/bookingappointment.md) in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt   |
|Anwendung | Nicht unterstützt  |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/appointments/{id}

```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.


## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "delete_bookingappointment"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
