---
title: Ressourcentyp bookingStaffMember
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 72130f46dc67d4491f9855706528ee5894b8352f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520277"
---
# <a name="bookingstaffmember-resource-type"></a>Ressourcentyp bookingStaffMember

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Stellt ein Mitarbeiter, die in einer [BookingBusiness](bookingbusiness.md)-Dienste bietet.

Mitarbeiter können Teil des Office-355 Mandanten sein, auf dem das Buchen Unternehmen konfiguriert ist, oder sie können e-Mail-Dienste von anderen e-Mail-Anbietern.

Beim Buchen von Terminen berücksichtigt die Buchungen API die folgenden Einstellungen, um ein Mitarbeiter Verfügbarkeit zu ermitteln: 

1. In der Standardeinstellung stellt den Betriebszeiten des Unternehmens (die **BusinessHours** -Eigenschaft der Entität [BookingBusiness](bookingbusiness.md) ) die allgemeine Verfügbarkeit des Mitarbeiters.
2. Wenn **UseBusinessHours** auf false festgelegt ist, stellt der Mitarbeiter bestimmte Arbeitsstunden (**WorkingHours** -Eigenschaft der Entität **BookingStaffmember** ) allgemeine Verfügbarkeit des Mitglieds an.
3. Wenn **AvailabilityIsAffectedByPersonalCalendar** auf true festgelegt ist, klicken Sie dann die Buchungen API würde zunächst sehen Sie sich die Mitarbeiter im Allgemeinen verfügbaren Stunden (wie von #1 oder 2 # bestimmt), und überprüfen Sie die Verfügbarkeit während der Stunden, die in der Mitarbeiter persönlich vor der Durchführung einer buchen Kalender.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste Mitarbeiter](../api/bookingbusiness-list-staffmembers.md) | [BookingStaffMember](bookingstaffmember.md) -Auflistung | Rufen Sie eine Liste der **BookingStaffMember** -Objekte in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md). |
|[Erstellen von bookingStaff](../api/bookingbusiness-post-staffmembers.md) | [BookingStaffMember](bookingstaffmember.md) -Auflistung | Erstellen Sie eine neue **BookingStaffMember** in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md). |
|[Abrufen von bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |Rufen Sie die Eigenschaften und Beziehungen zwischen einer **BookingStaffMember** in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).|
|[Update](../api/bookingstaffmember-update.md) | [bookingStaffMember](bookingstaffmember.md)    |Aktualisieren Sie die Eigenschaften einer **BookingStaffMember** in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).|
|[Delete](../api/bookingstaffmember-delete.md) | Keine |Löschen von Mitarbeitern in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Boolescher Wert|"True" bedeutet, dass, wenn der Mitarbeiter Office 365-Benutzer ist, der API Buchungen Verfügbarkeit der Mitarbeiter in ihre persönlichen Kalender auf Office 365, vergewissern Sie sich würde vor der Durchführung einer buchen. |
|ColorIndex|Int32|Identifiziert eine Farbe, um die Mitarbeiter darstellen. Die Farbe entspricht der Farbpalette in der Detailseite für **Mitarbeiter** in der app Buchungen.|
|displayName|String|Der Name des Mitarbeiters, wie Kunden angezeigt. Erforderlich.|
|emailAddress|String|Die e-Mail-Adresse des Mitarbeiters. Dies kann in der gleichen Office 365-Mandanten als das Unternehmen oder in eine andere e-Mail-Domäne sein. Diese e-Mail-Adresse kann verwendet werden, wenn die **SendConfirmationsToOwner** -Eigenschaft festgelegt ist, auf "true" in der scheduling Richtlinie des Unternehmens. Erforderlich.|
|id|Zeichenfolge| Die ID des Members Mitarbeiter in einer GUID-Format. Schreibgeschützt.|
|role|string| Die Rolle des Mitarbeiters im Unternehmen. Mögliche Werte: sind `guest`, `administrator`, `viewer` und `externalGuest`. Erforderlich.|
|useBusinessHours|Boolescher Wert|"True" bedeutet, dass die Mitarbeiter die Verfügbarkeit als ist in der **BusinessHours** -Eigenschaft des Unternehmens angegeben. False bedeutet, dass die Verfügbarkeit durch die Einstellung für die Mitarbeiter **WorkingHours** -Eigenschaft bestimmt wird.|
|workingHours|[BookingWorkHours](bookingworkhours.md) -Auflistung|Der Bereich der Stunden jeden Tag der Woche, die der Mitarbeiter für buchen verfügbar ist. Standardmäßig werden sie initialisiert, um die **BusinessHours** -Eigenschaft des Unternehmens identisch sein.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingStaffMember"
}-->

```json
{
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "role": "string",
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingstaffmember.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
