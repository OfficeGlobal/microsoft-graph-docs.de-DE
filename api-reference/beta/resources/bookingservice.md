---
title: Ressourcentyp bookingService
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 35e439888b39c81451242f01d2aaae89b65ad8ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519885"
---
# <a name="bookingservice-resource-type"></a>Ressourcentyp bookingService

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Stellt Informationen zu einem bestimmten Dienst stammt von einer [BookingBusiness](bookingbusiness.md), wie der Dienstname, Preis und die Mitarbeiter, die in der Regel ein solcher Dienst bereitstellt.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste Dienste](../api/bookingbusiness-list-services.md) | [BookingService](bookingservice.md) -Auflistung | Rufen Sie eine Liste der **BookingService** -Objekte in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).|
|[Erstellen von bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | Erstellen Sie eine **BookingService** für den angegebenen [Bookingbusiness](../resources/bookingbusiness.md). |
|[Abrufen von bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |Rufen Sie die Eigenschaften und die Beziehungen eines **BookingService** -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).|
|[Update](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |Aktualisieren eines **BookingService** -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md). |
|[Delete](../api/bookingservice-delete.md) | Keine |Löschen eines **BookingService** -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|defaultDuration|Dauer|Die standardmäßige Länge des Diensts, in der Anzahl von Tagen, Stunden, Minuten und Sekunden dargestellt. Beispielsweise P11D23H59M59.999999999999S. |
|defaultLocation|[location](location.md)|Der physische Standardspeicherort für den Dienst.|
|defaultPrice|Gleitkommawert mit doppelter Genauigkeit|Der Standardwert monetäre Preis für den Dienst.|
|defaultPriceType|string|Die Standardmethode der Dienst aufgeladen wird. Mögliche Werte sind: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs` und `notSet`.|
|defaultReminders|[BookingReminder](bookingreminder.md) -Auflistung|Die Standardeinstellung Festlegen von Erinnerungen für einen Termin dieses Diensts. Der Wert dieser Eigenschaft ist nur bei dieser **BookingService** anhand seiner ID Lesen verfügbar|
|description|String|Eine Beschreibung für den Dienst.|
|displayName|String|Ein Dienstname.|
|emailAddress|String|Eine E-Mail-Adresse:  |
|id|string|Die ID des Diensts aus, in einen GUID-Format. Schreibgeschützt.|
|isHiddenFromCustomers|Boolescher Wert|"True" bedeutet, dass dieser Dienst nicht verfügbar für Kunden für buchen ist.|
|notes|Zeichenfolge|Weitere Informationen zu diesem Dienst.|
|postBuffer|Dauer|Die Zeit bis zur Puffer nach eines Termins für diesen Dienst beendet, und vor dem nächsten Kunden Termin gebucht werden kann.|
|preBuffer|Dauer|Die Zeit zum Zwischenspeichern, bevor Sie ein Termin für diesen Dienst starten kann.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Der Satz von Richtlinien, die bestimmen, wie Termine für diesen Dienst erstellt und verwaltet werden soll.|
|staffMemberIds|Zeichenfolgenauflistung|Stellt die [Mitarbeiter](bookingstaffmember.md) , die diesen Dienst bereitzustellen. |

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": "string",
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "staffMemberIds": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingservice.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
