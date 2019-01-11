---
title: 'user: findMeetingTimes'
description: Schlagen Sie vor Besprechungszeiten und Speicherorte basierend auf der Organisator und Teilnehmer Verfügbarkeit und Zeit oder Ort Einschränkungen, die als Parameter angegeben.
localization_priority: Normal
ms.openlocfilehash: aae60b6148026725d325910c8c1ac0cd2ff376a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878911"
---
# <a name="user-findmeetingtimes"></a><span data-ttu-id="77a03-103">user: findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="77a03-103">user: findMeetingTimes</span></span>

> <span data-ttu-id="77a03-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="77a03-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77a03-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77a03-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77a03-106">Schlagen Sie vor Besprechungszeiten und Speicherorte basierend auf der Organisator und Teilnehmer Verfügbarkeit und Zeit oder Ort Einschränkungen, die als Parameter angegeben.</span><span class="sxs-lookup"><span data-stu-id="77a03-106">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints specified as parameters.</span></span>

<span data-ttu-id="77a03-p102">Wenn **findMeetingTimes** keine Besprechungsvorschläge zurückgeben kann, enthält die Antwort einen Grund, angegeben in der Eigenschaft **emptySuggestionsReason**. Ausgehend von diesem Wert können Sie die Parameter optimieren und **findMeetingTimes** erneut aufrufen.</span><span class="sxs-lookup"><span data-stu-id="77a03-p102">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>


## <a name="permissions"></a><span data-ttu-id="77a03-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="77a03-109">Permissions</span></span>
<span data-ttu-id="77a03-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77a03-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77a03-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77a03-112">Permission type</span></span>      | <span data-ttu-id="77a03-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77a03-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77a03-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77a03-114">Delegated (work or school account)</span></span> | <span data-ttu-id="77a03-115">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span><span class="sxs-lookup"><span data-stu-id="77a03-115">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span></span>    |
|<span data-ttu-id="77a03-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77a03-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77a03-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77a03-117">Not supported.</span></span>    |
|<span data-ttu-id="77a03-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77a03-118">Application</span></span> | <span data-ttu-id="77a03-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77a03-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77a03-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77a03-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a><span data-ttu-id="77a03-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77a03-121">Request headers</span></span>
| <span data-ttu-id="77a03-122">Name</span><span class="sxs-lookup"><span data-stu-id="77a03-122">Name</span></span>       | <span data-ttu-id="77a03-123">Wert</span><span class="sxs-lookup"><span data-stu-id="77a03-123">Value</span></span>|
|:---------------|:----------|
| <span data-ttu-id="77a03-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77a03-124">Authorization</span></span>  | <span data-ttu-id="77a03-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="77a03-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77a03-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="77a03-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="77a03-p105">Eine Zeichenfolge, die eine bestimmte Zeitzone für die Antwort darstellt, beispielsweise „Pacific Standard Time“. Optional. Wenn dieser Header nicht angegeben ist, wird UTC verwendet.</span><span class="sxs-lookup"><span data-stu-id="77a03-p105">A string representing a specific time zone for the response, for example, "Pacific Standard Time". Optional. UTC is used if this header is not specified.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77a03-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77a03-131">Request body</span></span>
<span data-ttu-id="77a03-p106">In der Tabelle unten sind alle unterstützten Parameter aufgeführt. Geben Sie abhängig von Ihrem jeweiligen Szenario für jeden notwendigen Parameter im Anforderungstext ein JSON-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="77a03-p106">All the supported parameters are listed below. Depending on your scenario, specify a JSON object for each of the necessary parameters in the request body.</span></span> 


| <span data-ttu-id="77a03-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="77a03-134">Parameter</span></span>    | <span data-ttu-id="77a03-135">Typ</span><span class="sxs-lookup"><span data-stu-id="77a03-135">Type</span></span>   |<span data-ttu-id="77a03-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="77a03-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77a03-137">attendees</span><span class="sxs-lookup"><span data-stu-id="77a03-137">attendees</span></span>|<span data-ttu-id="77a03-138">[attendeeBase](../resources/attendeebase.md) collection</span><span class="sxs-lookup"><span data-stu-id="77a03-138">[attendeeBase](../resources/attendeebase.md) collection</span></span>|<span data-ttu-id="77a03-p107">Eine Sammlung von Teilnehmern oder Ressourcen für die Besprechung. Da findMeetingTimes davon ausgeht, dass jeder Teilnehmer, bei dem es sich um eine Person handelt, immer erforderlich ist, geben Sie `required` für eine Person und `resource` für eine Ressource in der entsprechenden **type**-Eigenschaft an. Ist diese Sammlung leer, sucht **findMeetingTimes** nur für den Organisator nach freien Zeitfenstern. Optional.</span><span class="sxs-lookup"><span data-stu-id="77a03-p107">A collection of attendees or resources for the meeting. Since findMeetingTimes assumes that any attendee who is a person is always required, specify `required` for a person and `resource` for a resource in the corresponding **type** property. An empty collection causes **findMeetingTimes** to look for free time slots for only the organizer. Optional.</span></span>|
|<span data-ttu-id="77a03-143">isOrganizerOptional</span><span class="sxs-lookup"><span data-stu-id="77a03-143">isOrganizerOptional</span></span>|<span data-ttu-id="77a03-144">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="77a03-144">Edm.Boolean</span></span>|<span data-ttu-id="77a03-p108">Geben Sie `True` an, wenn der Organisator nicht zwingend teilnehmen muss. Der Standardwert lautet `false`. Optional.</span><span class="sxs-lookup"><span data-stu-id="77a03-p108">Specify `True` if the organizer doesn't necessarily have to attend. The default is `false`. Optional.</span></span>|
|<span data-ttu-id="77a03-148">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="77a03-148">locationConstraint</span></span>|[<span data-ttu-id="77a03-149">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="77a03-149">locationConstraint</span></span>](../resources/locationconstraint.md)|<span data-ttu-id="77a03-p109">Die Anforderungen des Organisators bezüglich des Besprechungsorts, z. B. ob ein Vorschlag für einen Besprechungsort erforderlich ist oder nur bestimmte Besprechungsorte zulässig sind. Optional.</span><span class="sxs-lookup"><span data-stu-id="77a03-p109">The organizer's requirements about the meeting location, such as whether a suggestion for a meeting location is required, or there are specific locations only where the meeting can take place. Optional.</span></span>|
|<span data-ttu-id="77a03-152">maxCandidates</span><span class="sxs-lookup"><span data-stu-id="77a03-152">maxCandidates</span></span>|<span data-ttu-id="77a03-153">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="77a03-153">Edm.Int32</span></span>|<span data-ttu-id="77a03-p110">Die maximale Anzahl an zurückgegebenen Besprechungsterminvorschlägen. Optional.</span><span class="sxs-lookup"><span data-stu-id="77a03-p110">The maximum number of meeting time suggestions to be returned. Optional.</span></span>|
|<span data-ttu-id="77a03-156">meetingDuration</span><span class="sxs-lookup"><span data-stu-id="77a03-156">meetingDuration</span></span>|<span data-ttu-id="77a03-157">Edm.Duration</span><span class="sxs-lookup"><span data-stu-id="77a03-157">Edm.Duration</span></span>|<span data-ttu-id="77a03-p111">Die Dauer der Besprechung im Format [ISO8601](https://www.iso.org/iso/iso8601). 1 Stunde wird beispielsweise als „PT1H“ angegeben. Dabei ist „P“ der Bezeichner für die Dauer, „T“ der Bezeichner für die Zeit und „H“ der Bezeichner für die Zeiteinheit Stunde. Verwenden Sie „M“ zum Angeben von Minuten für die Dauer. Beispiel: 2 Stunden und 30 Minuten wäre „PT2H30M“. Wenn keine Besprechungsdauer angegeben wird, verwendet **findMeetingTimes** den Standardwert von 30 Minuten. Optional.</span><span class="sxs-lookup"><span data-stu-id="77a03-p111">The length of the meeting, denoted in [ISO8601](https://www.iso.org/iso/iso8601) format. For example, 1 hour is denoted as 'PT1H', where 'P' is the duration designator, 'T' is the time designator, and 'H' is the hour designator. Use M to indicate minutes for the duration; for example, 2 hours and 30 minutes would be 'PT2H30M'. If no meeting duration is specified, **findMeetingTimes** uses the default of 30 minutes. Optional.</span></span>|
|<span data-ttu-id="77a03-163">minimumAttendeePercentage</span><span class="sxs-lookup"><span data-stu-id="77a03-163">minimumAttendeePercentage</span></span>|<span data-ttu-id="77a03-164">Edm.Double</span><span class="sxs-lookup"><span data-stu-id="77a03-164">Edm.Double</span></span>| <span data-ttu-id="77a03-p112">Die mindestens erforderliche [Konfidenz](#the-confidence-of-a-meeting-suggestion), damit ein bestimmtes Zeitfenster in der Antwort zurückgegeben wird. Hierbei handelt es sich um einen Prozentwert zwischen 0 und 100. Optional.</span><span class="sxs-lookup"><span data-stu-id="77a03-p112">The minimum required [confidence](#the-confidence-of-a-meeting-suggestion) for a time slot to be returned in the response. It is a % value ranging from 0 to 100. Optional.</span></span>|
|<span data-ttu-id="77a03-168">returnSuggestionReasons</span><span class="sxs-lookup"><span data-stu-id="77a03-168">returnSuggestionReasons</span></span>|<span data-ttu-id="77a03-169">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="77a03-169">Edm.Boolean</span></span>|<span data-ttu-id="77a03-p113">Geben Sie `True` an, wenn für jeden Besprechungsvorschlag ein Grund in der Eigenschaft **suggestionReason** zurückgegeben werden soll. Der Standardwert ist `false`, damit diese Eigenschaft nicht zurückgegeben wird. Optional.</span><span class="sxs-lookup"><span data-stu-id="77a03-p113">Specify `True` to return a reason for each meeting suggestion in the **suggestionReason** property. The default is `false` to not return that property. Optional.</span></span>|
|<span data-ttu-id="77a03-173">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="77a03-173">timeConstraint</span></span>|[<span data-ttu-id="77a03-174">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="77a03-174">timeConstraint</span></span>](../resources/timeconstraint.md)|<span data-ttu-id="77a03-p114">Alle Zeiteinschränkungen für eine Besprechung, z. B. die Art der Besprechung (Eigenschaft **activityDomain**) und mögliche Besprechungszeiträume (Eigenschaft **timeSlots**). **findMeetingTimes** geht davon aus, dass **activityDomain** auf `work` festgelegt ist, wenn Sie diesen Parameter nicht angeben. Optional.</span><span class="sxs-lookup"><span data-stu-id="77a03-p114">Any time restrictions for a meeting, which can include the nature of the meeting (**activityDomain** property) and possible meeting time periods (**timeSlots** property). **findMeetingTimes** assumes **activityDomain** as `work` if you don't specify this parameter. Optional.</span></span>|

<span data-ttu-id="77a03-178">In der folgenden Tabelle werden die Einschränkungen beschrieben, die Sie im Parameter **timeConstraint** genauer angeben können.</span><span class="sxs-lookup"><span data-stu-id="77a03-178">The following table describes the restrictions you can further specify in the **timeConstraint** parameter.</span></span>

|<span data-ttu-id="77a03-179">activityDomain-Wert in timeConstraint</span><span class="sxs-lookup"><span data-stu-id="77a03-179">activityDomain value in timeConstraint</span></span>|<span data-ttu-id="77a03-180">Vorschläge für Besprechungstermine</span><span class="sxs-lookup"><span data-stu-id="77a03-180">Suggestions for meeting times</span></span>|
|:-----|:-----|
|<span data-ttu-id="77a03-181">work</span><span class="sxs-lookup"><span data-stu-id="77a03-181">work</span></span>| <span data-ttu-id="77a03-p115">Vorschläge liegen innerhalb der Arbeitszeit des Benutzers, die in der Kalenderkonfiguration des Benutzers definiert wird, und können vom Benutzer oder Administrator angepasst werden. Die Standardarbeitszeit ist Montag bis Freitag von 08:00 Uhr bis 17:00 Uhr in der Zeitzone, die für das Postfach festgelegt ist. Dies ist der Standardwert, wenn keine **activityDomain** angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="77a03-p115">Suggestions are within the user's work hours which are defined in the user’s calendar configuration and can be customized by the user or administrator. The default work hours are Monday to Friday, 8am to 5pm in the time zone set for the mailbox. This is the default value if no **activityDomain** is specified.</span></span> |
|<span data-ttu-id="77a03-185">personal</span><span class="sxs-lookup"><span data-stu-id="77a03-185">personal</span></span>| <span data-ttu-id="77a03-p116">Vorschläge liegen innerhalb der Arbeitszeit des Benutzers sowie am Samstag und Sonntag. Der Standardwert ist Montag bis Sonntag von 08:00 Uhr bis 17:00 Uhr in der Zeitzone, die für das Postfach festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="77a03-p116">Suggestions are within the user's work hours, and Saturday and Sunday. The default is Monday to Sunday, 8am to 5pm, in the time zone setting for the mailbox.</span></span>|
|<span data-ttu-id="77a03-188">unrestricted</span><span class="sxs-lookup"><span data-stu-id="77a03-188">unrestricted</span></span> | <span data-ttu-id="77a03-189">Vorschläge können für jede Zeit des Tages an jedem Tag der Woche gemacht werden.</span><span class="sxs-lookup"><span data-stu-id="77a03-189">Suggestions can be from all hours of a day, all days of a week.</span></span>|
|<span data-ttu-id="77a03-190">unknown</span><span class="sxs-lookup"><span data-stu-id="77a03-190">unknown</span></span> | <span data-ttu-id="77a03-p117">Verwenden Sie diesen Wert nicht, da er in Zukunft veraltet sein wird. Aktuell verhält er sich genauso wie `work`. Ändern Sie vorhandenen Code so, dass er `work`, `personal` bzw. `unrestricted` verwendet.</span><span class="sxs-lookup"><span data-stu-id="77a03-p117">Do not use this value as it will be deprecated in the future. Currently behaves the same as `work`. Change any existing code to use `work`, `personal` or `unrestricted` as appropriate.</span></span>


<span data-ttu-id="77a03-p118">Ausgehend von den angegebenen Parametern überprüft **findMeetingTimes** den Frei-/Gebucht-Status im Hauptkalender des Organisators und in den Hauptkalendern der Teilnehmer. Die Aktion berechnet die bestmöglichen Besprechungstermine und gibt Besprechungsvorschläge zurück.</span><span class="sxs-lookup"><span data-stu-id="77a03-p118">Based on the specified parameters,**findMeetingTimes** checks the free/busy status in the primary calendars of the organizer and attendees. The action calculates the best possible meeting times, and returns any meeting suggestions.</span></span>

## <a name="response"></a><span data-ttu-id="77a03-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="77a03-196">Response</span></span>

<span data-ttu-id="77a03-197">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Ressource des Typs [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="77a03-197">If successful, this method returns `200 OK` response code and a [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) in the response body.</span></span> 

<span data-ttu-id="77a03-p119">Eine Ressource des Typs **meetingTimeSuggestionsResult** enthält eine Sammlung von Besprechungsvorschlägen und eine Eigenschaft **emptySuggestionsReason**. Jeder Vorschlag ist als eine Ressource des Typs [meetingTimeSuggestion](../resources/meetingtimesuggestion.md) definiert, für die die durchschnittliche Teilnahmekonfidenz der Teilnehmer bei 50 % oder einem spezifischen Prozentwert liegt, den Sie im Parameter **minimumAttendeePercentage** festgelegt haben.</span><span class="sxs-lookup"><span data-stu-id="77a03-p119">A **meetingTimeSuggestionsResult** includes a collection of meeting suggestions and an **emptySuggestionsReason** property. Each suggestion is defined as a [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), with attendees having on the average a confidence level of 50% to attend, or a specific % that you have specified in the **minimumAttendeePercentage** parameter.</span></span> 

<span data-ttu-id="77a03-200">Standardmäßig wird jeder Besprechungsterminvorschlag in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77a03-200">By default, each meeting time suggestion is returned in UTC.</span></span> 

<span data-ttu-id="77a03-p120">Wenn **findMeetingTimes** keine Besprechungsvorschläge zurückgeben kann, enthält die Antwort einen Grund, angegeben in der Eigenschaft **emptySuggestionsReason**. Ausgehend von diesem Wert können Sie die Parameter optimieren und **findMeetingTimes** erneut aufrufen.</span><span class="sxs-lookup"><span data-stu-id="77a03-p120">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

### <a name="the-confidence-of-a-meeting-suggestion"></a><span data-ttu-id="77a03-203">Die Konfidenz von Besprechungsvorschlägen</span><span class="sxs-lookup"><span data-stu-id="77a03-203">The confidence of a meeting suggestion</span></span>

<span data-ttu-id="77a03-204">Die Eigenschaft **confidence** einer Ressource des Typs **meetingTimeSuggestion** liegt in einem Bereich von 0 % bis 100 %. Sie gibt an, wie wahrscheinlich es ist, dass alle Teilnehmer an der Besprechung teilnehmen können, und basiert auf den Frei-/Gebucht-Status der einzelnen Teilnehmer:</span><span class="sxs-lookup"><span data-stu-id="77a03-204">The **confidence** property of a **meetingTimeSuggestion** ranges from 0% to 100%, and represents the chance that all the attendees attend the meeting, based on each of their individual free/busy status:</span></span>

- <span data-ttu-id="77a03-205">Für jeden Teilnehmer gilt: Ist der Status für eine Besprechung „Frei“, liegt die Teilnahmewahrscheinlichkeit bei 100 %. Beim Status „Unbekannt“ liegt sie bei 49 %, beim Status „Gebucht“ bei 0 %.</span><span class="sxs-lookup"><span data-stu-id="77a03-205">For each attendee, a free status for a specified meeting time period corresponds to 100% chance of attendance, unknown status 49%, and busy status 0%.</span></span>
- <span data-ttu-id="77a03-206">Zur Berechnung der Konfidenz eines Besprechungsterminvorschlags wird der Mittelwert aus den individuellen Teilnahmewahrscheinlichkeiten aller Besprechungsteilnehmer für die betreffende Besprechung gebildet.</span><span class="sxs-lookup"><span data-stu-id="77a03-206">The confidence of a meeting time suggestion is computed by averaging the chance of attendance over all the attendees specified for that meeting.</span></span>
- <span data-ttu-id="77a03-p121">Gibt es mehrere Besprechungsterminvorschläge, ordnet die Aktion **findMeetingTimes** die Vorschläge zunächst nach ihrem berechneten Konfidenzwert, beginnend mit dem Vorschlag mit dem höchsten Wert. Haben mehrere Vorschläge jeweils denselben Konfidenzwert, ordnet die Aktion diese Vorschläge chronologisch.</span><span class="sxs-lookup"><span data-stu-id="77a03-p121">If there are multiple meeting time suggestions, the **findMeetingTimes** action first orders the suggestions by their computed confidence value from high to low. If there are suggestions with the same confidence, the action then orders these suggestions chronologically.</span></span>
- <span data-ttu-id="77a03-p122">Mithilfe des optionalen Parameters **minimumAttendeePercentage** für **findMeetingTimes** können Sie festlegen, dass nur Besprechungsterminvorschläge mit einem bestimmten Mindestkonfidenzwert zurückgegeben werden. Beispielsweise können Sie eine **minimumAttendeePercentage** von 80 % festlegen, wenn Sie nur Vorschläge erhalten möchten, bei denen die Wahrscheinlichkeit, dass alle Teilnehmer teilnehmen können, bei mindestens 80 % liegt. Wenn Sie keine **minimumAttendeePercentage** festlegen, setzt **findMeetingTimes** einen Wert von 50 % an.</span><span class="sxs-lookup"><span data-stu-id="77a03-p122">You can use the **minimumAttendeePercentage** optional parameter for **findMeetingTimes** to specify only meeting time suggestions of at least certain confidence level should be returned. For example, you can specify a **minimumAttendeePercentage** of 80% if you want only suggestions that have an 80% chance or more that all the attendees are attending. If you do not specify **minimumAttendeePercentage**, **findMeetingTimes** assumes a value of 50%.</span></span>

<span data-ttu-id="77a03-212">Hier ein Beispiel für einen Besprechungsterminvorschlag für drei Teilnehmer mit folgendem Frei-/Gebucht-Status:</span><span class="sxs-lookup"><span data-stu-id="77a03-212">As an example, if a meeting time suggestion involves 3 attendees with the following free/busy status:</span></span>

|<span data-ttu-id="77a03-213">**Teilnehmer**</span><span class="sxs-lookup"><span data-stu-id="77a03-213">**Attendee**</span></span>|<span data-ttu-id="77a03-214">**Frei-/Gebucht-Status**</span><span class="sxs-lookup"><span data-stu-id="77a03-214">**Free/busy status**</span></span>|<span data-ttu-id="77a03-215">**Teilnahmewahrscheinlichkeit in %**</span><span class="sxs-lookup"><span data-stu-id="77a03-215">**% Chance of attendance**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="77a03-216">Dana</span><span class="sxs-lookup"><span data-stu-id="77a03-216">Dana</span></span> | <span data-ttu-id="77a03-217">Frei</span><span class="sxs-lookup"><span data-stu-id="77a03-217">Free</span></span> | <span data-ttu-id="77a03-218">100 %</span><span class="sxs-lookup"><span data-stu-id="77a03-218">100%</span></span> |
|<span data-ttu-id="77a03-219">John</span><span class="sxs-lookup"><span data-stu-id="77a03-219">John</span></span> | <span data-ttu-id="77a03-220">Unbekannt</span><span class="sxs-lookup"><span data-stu-id="77a03-220">Unknown</span></span> | <span data-ttu-id="77a03-221">49 %</span><span class="sxs-lookup"><span data-stu-id="77a03-221">49%</span></span> |
|<span data-ttu-id="77a03-222">Samantha</span><span class="sxs-lookup"><span data-stu-id="77a03-222">Samantha</span></span> | <span data-ttu-id="77a03-223">Gebucht</span><span class="sxs-lookup"><span data-stu-id="77a03-223">Busy</span></span> | <span data-ttu-id="77a03-224">0 %</span><span class="sxs-lookup"><span data-stu-id="77a03-224">0%</span></span> |

<span data-ttu-id="77a03-225">Die Konfidenz des Besprechungsterminvorschlags (durchschnittliche Teilnahmewahrscheinlichkeit) liegt hier bei (100 % + 49 % + 0 %) ÷ 3 = 49,66 %.</span><span class="sxs-lookup"><span data-stu-id="77a03-225">Then the confidence of the meeting time suggestion, which is the average chance of attendance, is (100% + 49% + 0%)/3 = 49.66%.</span></span>

<span data-ttu-id="77a03-226">Wenn Sie eine **minimumAttendeePercentage** von 80 % in einer Operation des Typs **findMeetingTimes** festlegen, wird die Operation diesen Termin nicht in der Antwort vorschlagen, da 49,66 % < 80 % ist.</span><span class="sxs-lookup"><span data-stu-id="77a03-226">If you specify a **minimumAttendeePercentage** of 80% in a **findMeetingTimes** operation, because 49.66% < 80%, the operation will not suggest this time in the response.</span></span>

## <a name="example"></a><span data-ttu-id="77a03-227">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77a03-227">Example</span></span>

<span data-ttu-id="77a03-228">Das folgende Beispiel veranschaulicht, wie Sie einen Besprechungstermin für einen vorab festgelegten Ort finden und für jeden Vorschlag einen Grund anfragen. Dazu geben Sie im Anforderungstext folgende Parameter an:</span><span class="sxs-lookup"><span data-stu-id="77a03-228">The following example shows how to find time to meet at a pre-determined location, and request a reason for each suggestion, by specifying the following parameters in the request body:</span></span>

- <span data-ttu-id="77a03-229">**attendees**</span><span class="sxs-lookup"><span data-stu-id="77a03-229">**attendees**</span></span>
- <span data-ttu-id="77a03-230">**locationConstraint**</span><span class="sxs-lookup"><span data-stu-id="77a03-230">**locationConstraint**</span></span>
- <span data-ttu-id="77a03-231">**timeConstraint**</span><span class="sxs-lookup"><span data-stu-id="77a03-231">**timeConstraint**</span></span>
- <span data-ttu-id="77a03-232">**meetingDuration**</span><span class="sxs-lookup"><span data-stu-id="77a03-232">**meetingDuration**</span></span>
- <span data-ttu-id="77a03-233">**returnSuggestionReasons**</span><span class="sxs-lookup"><span data-stu-id="77a03-233">**returnSuggestionReasons**</span></span>
- <span data-ttu-id="77a03-234">**minimumAttendeePercentage**</span><span class="sxs-lookup"><span data-stu-id="77a03-234">**minimumAttendeePercentage**</span></span>

<span data-ttu-id="77a03-235">Durch Setzen des Parameters **returnSuggestionReasons** wird für jeden Vorschlag auch eine Erklärung in der Eigenschaft **suggestionReason** vermerkt, sofern **findMeetingTimes** Vorschläge zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="77a03-235">By setting the **returnSuggestionReasons** parameter, you also get an explanation in the **suggestionReason** property for each suggestion, if **findMeetingTimes** returns any suggestion.</span></span>

<span data-ttu-id="77a03-p123">Beachten Sie: In der Anforderung gilt für die Zeit die Zeitzone PST. Die Antwort gibt Besprechungsterminvorschläge jedoch standardmäßig in UTC zurück. Sie können den Anforderungsheader `Prefer: outlook.timezone` verwenden, um auch für die Zeitwerte in der Antwort die Zeitzone PST festzulegen.</span><span class="sxs-lookup"><span data-stu-id="77a03-p123">Notice that the request specifies time in the PST time zone, and the response returns meeting time suggestions in UTC, by default. You can use the `Prefer: outlook.timezone` request header to specify PST as well for the time values in the response.</span></span>

##### <a name="request"></a><span data-ttu-id="77a03-238">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77a03-238">Request</span></span>
<span data-ttu-id="77a03-239">Hier sehen Sie die Beispielanforderung:</span><span class="sxs-lookup"><span data-stu-id="77a03-239">Here is the example request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/beta/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": "false",  
    "suggestLocation": "false",  
    "locations": [ 
      { 
        "resolveAvailability": "false",
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"unrestricted", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-17T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-19T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "100"
}
```

##### <a name="response"></a><span data-ttu-id="77a03-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="77a03-240">Response</span></span>
<span data-ttu-id="77a03-p124">Unten sehen Sie eine Beispielantwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77a03-p124">Here is an example response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 976

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"",
    "meetingTimeSuggestions":[
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T18:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        },
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T22:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/beta/api/user_findmeetingtimes.md:
      Failed to parse any rows out of table with headers: |activityDomain value|Suggestions for meeting times|"
  ],
  "tocPath": ""
}-->
