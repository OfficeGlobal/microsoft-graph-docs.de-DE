---
title: Bookingservice aktualisieren
description: Aktualisieren Sie die Eigenschaften eines BookingService-Objekts in der angegebenen Bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6049fe68eaa45597246bef1c1b11952e3c4a5d42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519717"
---
# <a name="update-bookingservice"></a>Bookingservice aktualisieren

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie die Eigenschaften eines [BookingService](../resources/bookingservice.md) -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).

Es folgen einige Beispiele, die Sie für einen Dienst anpassen können:
- Kurs
- Typische Länge eines Termins
- Erinnerungen
- Jedes Mal, wenn Puffer, richten Sie vor oder nach der Service abschließen
- [Planen von Richtlinien](../resources/bookingschedulingpolicy.md) Parameter wie minimale Hinweis zum Buch oder Abbrechen, und ob Kunden bestimmte Mitarbeiter für einen Termin auswählen können.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  Bookings.ReadWrite.All Bookings.Manage.All   |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt   |
|Anwendung | Nicht unterstützt  |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a>Optionale Anforderungsheader
| Name       | Beschreibung|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|defaultDuration|Dauer|Die standardmäßige Länge des Diensts, in der Anzahl von Tagen, Stunden, Minuten und Sekunden dargestellt. Beispielsweise P11D23H59M59.999999999999S. |
|defaultLocation|[location](../resources/location.md)|Der physische Standardspeicherort für den Dienst.|
|defaultPrice|Gleitkommawert mit doppelter Genauigkeit|Der Standardwert monetäre Preis für den Dienst.|
|defaultPriceType|string|Die Standardmethode der Dienst aufgeladen wird. Mögliche Werte sind: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs` und `notSet`.|
|defaultReminders|[BookingReminder](../resources/bookingreminder.md) -Auflistung|Die Standardeinstellung Festlegen von Erinnerungen für einen Termin dieses Diensts. Der Wert dieser Eigenschaft ist nur bei dieser **BookingService** anhand seiner ID Lesen verfügbar|
|description|String|Eine Beschreibung für den Dienst.|
|displayName|String|Ein Dienstname.|
|emailAddress|String|Eine E-Mail-Adresse:  |
|id|String| Schreibgeschützt.|
|isHiddenFromCustomers|Boolescher Wert|"True" bedeutet, dass dieser Dienst nicht verfügbar für Kunden für buchen ist.|
|notes|Zeichenfolge|Weitere Informationen zu diesem Dienst.|
|postBuffer|Dauer|Die Zeit bis zur Puffer nach eines Termins für diesen Dienst beendet, und vor dem nächsten Kunden Termin gebucht werden kann.|
|preBuffer|Dauer|Die Zeit zum Zwischenspeichern, bevor Sie ein Termin für diesen Dienst starten kann.|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|Der Satz von Richtlinien, die bestimmen, wie Termine für diesen Dienst erstellt und verwaltet werden soll.|
|staffMemberIds|Zeichenfolgenauflistung|Stellt die [Mitarbeiter](../resources/bookingstaffmember.md) , die diesen Dienst bereitzustellen. |

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Im folgende Beispiel wird die Dauer des angegebenen Dienstes aktualisiert.
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
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
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
