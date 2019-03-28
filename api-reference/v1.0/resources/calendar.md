---
title: Ressourcentyp calendar
description: Ein Kalender, der ein Container für Ereignisse ist. Dies kann ein Kalender für einen Benutzer oder der Standardkalender einer Office 365-Gruppe sein.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1ca76ba581b4db8ab3a42ccc993e545afd9a922c
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936311"
---
# <a name="calendar-resource-type"></a>Ressourcentyp calendar

Ein Kalender, der ein Container für Ereignisse ist. Dies kann ein Kalender für einen [Benutzer](user.md) oder der Standardkalender einer Office 365-[Gruppe](group.md) sein.

> **Hinweis:** Es gibt einige kleinere Unterschiede in der Weise, wie Sie mit Benutzerkalendern und Gruppenkalendern interagieren können:

 - Benutzerkalender können Sie nur in einer [CalendarGroup](calendargroup.md) organisieren.
 - Outlook akzeptiert automatisch alle Besprechungsanfragen im Auftrag von Gruppen. Das [Annehmen](../api/event-accept.md), [Mit Vorbehalt annehmen](../api/event-tentativelyaccept.md) oder [Ablehnen](../api/event-decline.md) von Besprechungsanfragen ist nur bei Benutzerkalendern möglich.
  - Outlook unterstützt keine Erinnerungen für Gruppenereignisse. Das [Erneute Erinnern](../api/event-snoozereminder.md) oder [Schließen](../api/event-dismissreminder.md) einer [Erinnerung](reminder.md) ist nur bei Benutzerkalendern möglich.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Kalender auflisten](../api/user-list-calendars.md)|[calender](calendar.md)-Sammlung|Rufen Sie alle Kalender des Benutzers oder die Kalender auf der Standardgruppe oder einer anderen bestimmten Kalendergruppe ab.|
|[Kalender erstellen](../api/user-post-calendars.md) |[Kalender](calendar.md)| Erstellen Sie einen neuen Kalender in der Standardkalendergruppe oder in der angegebenen Kalendergruppe für einen Benutzer.|
|[Kalender abrufen](../api/calendar-get.md) | [Kalender](calendar.md) |Dient zum Abrufen der Eigenschaften und der Beziehungen eines **calendar**-Objekts. Dies kann ein Kalender für einen Benutzer oder der Standardkalender einer Office 365-Gruppe sein. |
|[Aktualisieren](../api/calendar-update.md) | [Kalender](calendar.md)  |Mit dieser API können Sie die Eigenschaften eines **calendar**-Objekts aktualisieren. Dies kann ein Kalender für einen Benutzer oder der Standardkalender einer Office 365-Gruppe sein. |
|[Löschen](../api/calendar-delete.md) | Keine |Dient zum Löschen des Kalenderobjekts aktualisieren. |
|[calendarView auflisten](../api/calendar-list-calendarview.md) |[Ereignissammlung](event.md)| Dient zum Abrufen der Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer Kalenderansicht, die durch eine Zeitbereich definiert werden, aus dem primären Kalender `(../me/calendarview)` des Benutzers oder aus einem angegebenen Kalender.|
|[Ereignisse auflisten](../api/calendar-list-events.md) |[Ereignissammlung](event.md)| Dient zum Abrufen einer Liste von Ereignissen in einem Kalender. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.|
|[Ereignis erstellen](../api/calendar-post-events.md) |[event](event.md)| Dient zum Erstellen eines neuen Ereignisses im Standardkalender oder im angegebenen Kalender.|
|[getSchedule](../api/calendar-getschedule.md) |[scheduleInformation](scheduleinformation.md)-Sammlung|Rufen Sie die Frei/Gebucht-Informationen zur Verfügbarkeit von Benutzern, Verteilerlisten oder Ressourcen für einen angegebenen Zeitraum ab. |
|[findMeetingTimes](../api/user-findmeetingtimes.md) |[meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) |Schlägt Besprechungszeiten und -orte basierend auf der Verfügbarkeit des Organisators und der Teilnehmer sowie auf spezifizierten Zeit- oder Ortseinschränkungen vor. |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[Kalender](calendar.md)  |Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen Kalender.   |
|[Kalender mit einwertiger erweiterter Eigenschaft abrufen](../api/singlevaluelegacyextendedproperty-get.md)  | [Kalender](calendar.md) | Ruft mithilfe von `$expand` oder `$filter` Kalender mit einer einwertigen erweiterten Eigenschaft ab. |
|[Mehrwertige erweiterte Eigenschaft erstellen](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [Kalender](calendar.md) | Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen Kalender.  |
|[Kalender mit mehrwertiger erweiterter Eigenschaft abrufen](../api/multivaluelegacyextendedproperty-get.md)  | [Kalender](calendar.md) | Dient zum Abrufen eines Kalenders mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|canEdit |Boolescher Wert |„True“, wenn der Benutzer in den Kalender schreiben kann, andernfalls „false“. Diese Eigenschaft ist für den Benutzer, der den Kalender erstellt hat, „true“. Diese Eigenschaft ist auch für einen Benutzer „true“, für den ein Kalender freigegeben wurde und der Schreibzugriff hat. |
|canShare |Boolescher Wert |„True“, wenn der Benutzer die Berechtigung zum Freigeben des Kalenders hat, andernfalls „false“. Nur der Benutzer, der den Kalender erstellt hat, kann ihn freigeben. |
|canViewPrivateItems |Boolean |„True“, wenn der Benutzer Elemente im Kalender lesen kann, die als „privat“ markiert wurden, andernfalls „false“. |
|changeKey|Zeichenfolge|Gibt die Version des Kalenderobjekts an. Jedes Mal, wenn der Kalender geändert wird, wird auch „changeKey“ geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen. Schreibgeschützt.|
|color|calendarColor|Gibt das Farbdesign an, um den Kalender von anderen Kalendern in einer Benutzeroberfläche zu unterscheiden. Die Eigenschaftswerte sind: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1|
|id|String|Eindeutiger Bezeichner für die Gruppe. Schreibgeschützt.|
|name|String|Der Kalendername.|
|owner |[emailAddress](emailaddress.md) | Wenn festgelegt, stellt dies den Benutzer dar, der den Kalender erstellt oder hinzugefügt hat. Für einen Kalender, den der Benutzer erstellt oder hinzugefügt hat, wird die Eigenschaft **owner** auf den Benutzer festgelegt. Für einen Kalender, der für den Benutzer freigegeben wurde, wird die Eigenschaft **owner** auf die Person festgelegt, die den Kalender für den Benutzer freigegeben hat. |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|calendarView|[Ereignissammlung](event.md)|Die Kalenderansicht für den Kalender. Navigationseigenschaft. Schreibgeschützt.|
|events|[Ereignissammlung](event.md)|Die Ereignisse im Kalender. Navigationseigenschaft. Schreibgeschützt.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter mehrwertiger Eigenschaften, die für den Kalender definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter einwertiger Eigenschaften, die für den Kalender definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendar",
  "@odata.annotations": [
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
