---
title: Ressourcentyp calendar
description: Ein Kalender, der ein Container für Ereignisse ist. Dies kann ein Kalender für einen Benutzer oder der Standardkalender einer Office 365-Gruppe sein.
localization_priority: Priority
ms.openlocfilehash: c567a37be651987f2ca5af08cf9837ba6f41076f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843246"
---
# <a name="calendar-resource-type"></a><span data-ttu-id="d77cb-104">Ressourcentyp calendar</span><span class="sxs-lookup"><span data-stu-id="d77cb-104">calendar resource type</span></span>

<span data-ttu-id="d77cb-105">Ein Kalender, der ein Container für Ereignisse ist.</span><span class="sxs-lookup"><span data-stu-id="d77cb-105">A calendar which is a container for events.</span></span> <span data-ttu-id="d77cb-106">Dies kann ein Kalender für einen [Benutzer](user.md) oder der Standardkalender einer Office 365-[Gruppe](group.md) sein.</span><span class="sxs-lookup"><span data-stu-id="d77cb-106">It can be a calendar for a [user](user.md), or the default calendar of an Office 365 [group](group.md).</span></span>

> <span data-ttu-id="d77cb-107">**Hinweis:** Es gibt einige kleinere Unterschiede bei der Verarbeitung von Benutzerkalender und Gruppenkalender interagieren können:</span><span class="sxs-lookup"><span data-stu-id="d77cb-107">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

 - <span data-ttu-id="d77cb-108">Sie können nur Benutzerkalender in einer [CalendarGroup](calendargroup.md)organisieren.</span><span class="sxs-lookup"><span data-stu-id="d77cb-108">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
 - <span data-ttu-id="d77cb-109">Outlook akzeptiert automatisch alle Besprechungsanfragen für Gruppen.</span><span class="sxs-lookup"><span data-stu-id="d77cb-109">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="d77cb-110">Sie können für Benutzerkalender nur [annehmen](../api/event-accept.md), [mit Vorbehalt annehmen](../api/event-tentativelyaccept.md)oder [Ablehnen](../api/event-decline.md) von Besprechungsanfragen.</span><span class="sxs-lookup"><span data-stu-id="d77cb-110">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for user calendars only.</span></span>
  - <span data-ttu-id="d77cb-111">Outlook unterstützt keine Erinnerungen für Ereignisse gruppieren.</span><span class="sxs-lookup"><span data-stu-id="d77cb-111">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="d77cb-112">Sie können für Benutzerkalender nur [erneut erinnern](../api/event-snoozereminder.md) oder eine [Erinnerung](reminder.md) [zu schließen](../api/event-dismissreminder.md) .</span><span class="sxs-lookup"><span data-stu-id="d77cb-112">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="d77cb-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="d77cb-113">Methods</span></span>

| <span data-ttu-id="d77cb-114">Methode</span><span class="sxs-lookup"><span data-stu-id="d77cb-114">Method</span></span>       | <span data-ttu-id="d77cb-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d77cb-115">Return Type</span></span>  |<span data-ttu-id="d77cb-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d77cb-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d77cb-117">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="d77cb-117">List calendars</span></span>](../api/user-list-calendars.md)|<span data-ttu-id="d77cb-118">[calender](calendar.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d77cb-118">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="d77cb-119">Rufen Sie alle Kalender des Benutzers oder die Kalender auf der Standardgruppe oder einer anderen bestimmten Kalendergruppe ab.</span><span class="sxs-lookup"><span data-stu-id="d77cb-119">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="d77cb-120">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="d77cb-120">Create calendar</span></span>](../api/user-post-calendars.md) |[<span data-ttu-id="d77cb-121">Kalender</span><span class="sxs-lookup"><span data-stu-id="d77cb-121">calendar</span></span>](calendar.md)| <span data-ttu-id="d77cb-122">Erstellen Sie einen neuen Kalender in der Standardkalendergruppe oder in der angegebenen Kalendergruppe für einen Benutzer.</span><span class="sxs-lookup"><span data-stu-id="d77cb-122">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="d77cb-123">Kalender abrufen</span><span class="sxs-lookup"><span data-stu-id="d77cb-123">Get calendar</span></span>](../api/calendar-get.md) | [<span data-ttu-id="d77cb-124">Kalender</span><span class="sxs-lookup"><span data-stu-id="d77cb-124">calendar</span></span>](calendar.md) |<span data-ttu-id="d77cb-125">Dient zum Abrufen der Eigenschaften und der Beziehungen eines **calendar**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d77cb-125">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="d77cb-126">Dies kann ein Kalender für einen Benutzer oder der Standardkalender einer Office 365-Gruppe sein.</span><span class="sxs-lookup"><span data-stu-id="d77cb-126">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="d77cb-127">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d77cb-127">Update</span></span>](../api/calendar-update.md) | [<span data-ttu-id="d77cb-128">Kalender</span><span class="sxs-lookup"><span data-stu-id="d77cb-128">calendar</span></span>](calendar.md)  |<span data-ttu-id="d77cb-129">Mit dieser API können Sie die Eigenschaften eines **calendar**-Objekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="d77cb-129">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="d77cb-130">Dies kann ein Kalender für einen Benutzer oder der Standardkalender einer Office 365-Gruppe sein.</span><span class="sxs-lookup"><span data-stu-id="d77cb-130">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="d77cb-131">Löschen</span><span class="sxs-lookup"><span data-stu-id="d77cb-131">Delete</span></span>](../api/calendar-delete.md) | <span data-ttu-id="d77cb-132">Keine</span><span class="sxs-lookup"><span data-stu-id="d77cb-132">None</span></span> |<span data-ttu-id="d77cb-133">Dient zum Löschen des Kalenderobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="d77cb-133">Delete calendar object.</span></span> |
|[<span data-ttu-id="d77cb-134">calendarView auflisten</span><span class="sxs-lookup"><span data-stu-id="d77cb-134">List calendarView</span></span>](../api/calendar-list-calendarview.md) |<span data-ttu-id="d77cb-135">[Ereignissammlung](event.md)</span><span class="sxs-lookup"><span data-stu-id="d77cb-135">[event](event.md) collection</span></span>| <span data-ttu-id="d77cb-136">Dient zum Abrufen der Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer Kalenderansicht, die durch eine Zeitbereich definiert werden, aus dem primären Kalender `(../me/calendarview)` des Benutzers oder aus einem angegebenen Kalender.</span><span class="sxs-lookup"><span data-stu-id="d77cb-136">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="d77cb-137">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="d77cb-137">List events</span></span>](../api/calendar-list-events.md) |<span data-ttu-id="d77cb-138">[Ereignissammlung](event.md)</span><span class="sxs-lookup"><span data-stu-id="d77cb-138">[event](event.md) collection</span></span>| <span data-ttu-id="d77cb-p107">Dient zum Abrufen einer Liste von Ereignissen in einem Kalender.  Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.</span><span class="sxs-lookup"><span data-stu-id="d77cb-p107">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="d77cb-141">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="d77cb-141">Create event</span></span>](../api/calendar-post-events.md) |[<span data-ttu-id="d77cb-142">Ereignis</span><span class="sxs-lookup"><span data-stu-id="d77cb-142">event</span></span>](event.md)| <span data-ttu-id="d77cb-143">Erstellen Sie ein neues Ereignis in die standardmäßigen oder den angegebenen Kalender.</span><span class="sxs-lookup"><span data-stu-id="d77cb-143">Create a new event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="d77cb-144">findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="d77cb-144">findMeetingTimes</span></span>](../api/user-findmeetingtimes.md) |[<span data-ttu-id="d77cb-145">meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="d77cb-145">meetingTimeSuggestionsResult</span></span>](meetingtimesuggestionsresult.md) |<span data-ttu-id="d77cb-146">Schlagen Sie vor Besprechungszeiten und Speicherorte basierend auf der Organisator und Teilnehmer Verfügbarkeit und Zeit oder Ort Einschränkungen.</span><span class="sxs-lookup"><span data-stu-id="d77cb-146">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints.</span></span> |
|[<span data-ttu-id="d77cb-147">Einwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="d77cb-147">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="d77cb-148">Kalender</span><span class="sxs-lookup"><span data-stu-id="d77cb-148">calendar</span></span>](calendar.md)  |<span data-ttu-id="d77cb-149">Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen Kalender.</span><span class="sxs-lookup"><span data-stu-id="d77cb-149">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="d77cb-150">Kalender mit einwertiger erweiterter Eigenschaft abrufen</span><span class="sxs-lookup"><span data-stu-id="d77cb-150">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="d77cb-151">Kalender</span><span class="sxs-lookup"><span data-stu-id="d77cb-151">calendar</span></span>](calendar.md) | <span data-ttu-id="d77cb-152">Ruft mithilfe von `$expand` oder `$filter` Kalender mit einer einwertigen erweiterten Eigenschaft ab.</span><span class="sxs-lookup"><span data-stu-id="d77cb-152">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="d77cb-153">Mehrwertige erweiterte Eigenschaft erstellen</span><span class="sxs-lookup"><span data-stu-id="d77cb-153">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="d77cb-154">Kalender</span><span class="sxs-lookup"><span data-stu-id="d77cb-154">calendar</span></span>](calendar.md) | <span data-ttu-id="d77cb-155">Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen Kalender.</span><span class="sxs-lookup"><span data-stu-id="d77cb-155">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="d77cb-156">Kalender mit mehrwertiger erweiterter Eigenschaft abrufen</span><span class="sxs-lookup"><span data-stu-id="d77cb-156">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="d77cb-157">Kalender</span><span class="sxs-lookup"><span data-stu-id="d77cb-157">calendar</span></span>](calendar.md) | <span data-ttu-id="d77cb-158">Dient zum Abrufen eines Kalenders mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`.</span><span class="sxs-lookup"><span data-stu-id="d77cb-158">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="d77cb-159">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d77cb-159">Properties</span></span>
| <span data-ttu-id="d77cb-160">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d77cb-160">Property</span></span>     | <span data-ttu-id="d77cb-161">Typ</span><span class="sxs-lookup"><span data-stu-id="d77cb-161">Type</span></span>   |<span data-ttu-id="d77cb-162">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d77cb-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d77cb-163">canEdit</span><span class="sxs-lookup"><span data-stu-id="d77cb-163">canEdit</span></span> |<span data-ttu-id="d77cb-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="d77cb-164">Boolean</span></span> |<span data-ttu-id="d77cb-p108">„True“, wenn der Benutzer in den Kalender schreiben kann, andernfalls „false“. Diese Eigenschaft ist für den Benutzer, der den Kalender erstellt hat, „true“. Diese Eigenschaft ist auch für einen Benutzer „true“, für den ein Kalender freigegeben wurde und der Schreibzugriff hat.</span><span class="sxs-lookup"><span data-stu-id="d77cb-p108">True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="d77cb-168">canShare</span><span class="sxs-lookup"><span data-stu-id="d77cb-168">canShare</span></span> |<span data-ttu-id="d77cb-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="d77cb-169">Boolean</span></span> |<span data-ttu-id="d77cb-p109">„True“, wenn der Benutzer die Berechtigung zum Freigeben des Kalenders hat, andernfalls „false“. Nur der Benutzer, der den Kalender erstellt hat, kann ihn freigeben.</span><span class="sxs-lookup"><span data-stu-id="d77cb-p109">True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="d77cb-172">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="d77cb-172">canViewPrivateItems</span></span> |<span data-ttu-id="d77cb-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="d77cb-173">Boolean</span></span> |<span data-ttu-id="d77cb-174">„True“, wenn der Benutzer Elemente im Kalender lesen kann, die als „privat“ markiert wurden, andernfalls „false“.</span><span class="sxs-lookup"><span data-stu-id="d77cb-174">True if the user can read calendar items that have been marked private, false otherwise.</span></span> |
|<span data-ttu-id="d77cb-175">changeKey</span><span class="sxs-lookup"><span data-stu-id="d77cb-175">changeKey</span></span>|<span data-ttu-id="d77cb-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d77cb-176">String</span></span>|<span data-ttu-id="d77cb-p110">Gibt die Version des Kalenderobjekts an. Jedes Mal, wenn der Kalender geändert wird, wird auch „changeKey“ geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d77cb-p110">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="d77cb-181">color</span><span class="sxs-lookup"><span data-stu-id="d77cb-181">color</span></span>|<span data-ttu-id="d77cb-182">calendarColor</span><span class="sxs-lookup"><span data-stu-id="d77cb-182">calendarColor</span></span>|<span data-ttu-id="d77cb-p111">Gibt das Farbdesign an, um den Kalender von anderen Kalendern in einer Benutzeroberfläche zu unterscheiden. Die Eigenschaftswerte sind: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="d77cb-p111">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="d77cb-185">id</span><span class="sxs-lookup"><span data-stu-id="d77cb-185">id</span></span>|<span data-ttu-id="d77cb-186">String</span><span class="sxs-lookup"><span data-stu-id="d77cb-186">String</span></span>|<span data-ttu-id="d77cb-p112">Eindeutiger Bezeichner für die Gruppe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d77cb-p112">The group's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="d77cb-189">name</span><span class="sxs-lookup"><span data-stu-id="d77cb-189">name</span></span>|<span data-ttu-id="d77cb-190">String</span><span class="sxs-lookup"><span data-stu-id="d77cb-190">String</span></span>|<span data-ttu-id="d77cb-191">Der Kalendername.</span><span class="sxs-lookup"><span data-stu-id="d77cb-191">The calendar name.</span></span>|
|<span data-ttu-id="d77cb-192">owner</span><span class="sxs-lookup"><span data-stu-id="d77cb-192">owner</span></span> |[<span data-ttu-id="d77cb-193">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d77cb-193">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="d77cb-p113">Wenn festgelegt, stellt dies den Benutzer dar, der den Kalender erstellt oder hinzugefügt hat. Für einen Kalender, den der Benutzer erstellt oder hinzugefügt hat, wird die Eigenschaft **owner** auf den Benutzer festgelegt. Für einen Kalender, der für den Benutzer freigegeben wurde, wird die Eigenschaft **owner** auf die Person festgelegt, die den Kalender für den Benutzer freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="d77cb-p113">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d77cb-197">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d77cb-197">Relationships</span></span>
| <span data-ttu-id="d77cb-198">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d77cb-198">Relationship</span></span> | <span data-ttu-id="d77cb-199">Typ</span><span class="sxs-lookup"><span data-stu-id="d77cb-199">Type</span></span>   |<span data-ttu-id="d77cb-200">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d77cb-200">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d77cb-201">calendarView</span><span class="sxs-lookup"><span data-stu-id="d77cb-201">calendarView</span></span>|<span data-ttu-id="d77cb-202">[Ereignissammlung](event.md)</span><span class="sxs-lookup"><span data-stu-id="d77cb-202">[Event](event.md) collection</span></span>|<span data-ttu-id="d77cb-p114">Die Kalenderansicht für den Kalender. Navigationseigenschaft. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d77cb-p114">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="d77cb-206">events</span><span class="sxs-lookup"><span data-stu-id="d77cb-206">events</span></span>|<span data-ttu-id="d77cb-207">[Ereignissammlung](event.md)</span><span class="sxs-lookup"><span data-stu-id="d77cb-207">[Event](event.md) collection</span></span>|<span data-ttu-id="d77cb-p115">Die Ereignisse im Kalender. Navigationseigenschaft. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d77cb-p115">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="d77cb-211">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d77cb-211">multiValueExtendedProperties</span></span>|<span data-ttu-id="d77cb-212">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d77cb-212">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d77cb-p116">Die Sammlung erweiterter mehrwertiger Eigenschaften, die für den Kalender definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="d77cb-p116">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d77cb-216">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d77cb-216">singleValueExtendedProperties</span></span>|<span data-ttu-id="d77cb-217">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d77cb-217">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d77cb-p117">Die Sammlung erweiterter einwertiger Eigenschaften, die für den Kalender definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="d77cb-p117">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d77cb-221">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d77cb-221">JSON representation</span></span>

<span data-ttu-id="d77cb-222">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d77cb-222">Here is a JSON representation of the resource</span></span>

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
