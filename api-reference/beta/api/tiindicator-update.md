---
title: TiIndicator aktualisieren
description: Aktualisieren der Eigenschaften eines tiIndicator-Objekts.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 3c7ec883be4d84efa028362438660ade38e23689
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30367085"
---
# <a name="update-tiindicator"></a><span data-ttu-id="6d640-103">TiIndicator aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6d640-103">Update tiIndicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d640-104">Aktualisieren der Eigenschaften eines [tiIndicator](../resources/tiindicator.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6d640-104">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d640-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6d640-105">Permissions</span></span>

<span data-ttu-id="6d640-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d640-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d640-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d640-108">Permission type</span></span>                        | <span data-ttu-id="6d640-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d640-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6d640-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d640-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d640-111">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="6d640-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="6d640-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d640-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d640-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d640-113">Not supported.</span></span> |
| <span data-ttu-id="6d640-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d640-114">Application</span></span>                            | <span data-ttu-id="6d640-115">ThreatIndicators. ReadWrite. OwnedBy</span><span class="sxs-lookup"><span data-stu-id="6d640-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d640-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d640-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6d640-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d640-117">Request headers</span></span>

| <span data-ttu-id="6d640-118">Name</span><span class="sxs-lookup"><span data-stu-id="6d640-118">Name</span></span>       | <span data-ttu-id="6d640-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d640-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6d640-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d640-120">Authorization</span></span> | <span data-ttu-id="6d640-121">Bearer {Code} **erforderlich**</span><span class="sxs-lookup"><span data-stu-id="6d640-121">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="6d640-122">Prefer</span><span class="sxs-lookup"><span data-stu-id="6d640-122">Prefer</span></span> | <span data-ttu-id="6d640-123">Return = Darstellung</span><span class="sxs-lookup"><span data-stu-id="6d640-123">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d640-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d640-124">Request body</span></span>

<span data-ttu-id="6d640-125">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6d640-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6d640-126">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="6d640-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6d640-127">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="6d640-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6d640-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d640-128">Property</span></span>     | <span data-ttu-id="6d640-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6d640-129">Type</span></span>        | <span data-ttu-id="6d640-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d640-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6d640-131">Aktion</span><span class="sxs-lookup"><span data-stu-id="6d640-131">action</span></span>|<span data-ttu-id="6d640-132">string</span><span class="sxs-lookup"><span data-stu-id="6d640-132">string</span></span>| <span data-ttu-id="6d640-133">Die Aktion, die angewendet werden soll, wenn das Symbol im targetProduct-Sicherheitstool abgeglichen wird.</span><span class="sxs-lookup"><span data-stu-id="6d640-133">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="6d640-134">Mögliche Werte: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="6d640-134">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="6d640-135">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="6d640-135">activityGroupNames</span></span>|<span data-ttu-id="6d640-136">String collection</span><span class="sxs-lookup"><span data-stu-id="6d640-136">String collection</span></span>|<span data-ttu-id="6d640-137">Die Namen der Cyber Threat Intelligence für die Parteien, die für die bösartigen Aktivitäten verantwortlich sind, die vom Bedrohungs Indikator erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="6d640-137">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="6d640-138">Zusatzinformationen</span><span class="sxs-lookup"><span data-stu-id="6d640-138">additionalInformation</span></span>|<span data-ttu-id="6d640-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d640-139">String</span></span>|<span data-ttu-id="6d640-140">Ein CatchAll Bereich, in dem zusätzliche Daten aus dem Indikator, die nicht von anderen tiIndicator-Eigenschaften abgedeckt werden, möglicherweise eingefügt werden.</span><span class="sxs-lookup"><span data-stu-id="6d640-140">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="6d640-141">Daten, die in Zusatzinformationen werden, werden in der Regel nicht vom targetProduct-Sicherheitstool verwendet.</span><span class="sxs-lookup"><span data-stu-id="6d640-141">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="6d640-142">confidence</span><span class="sxs-lookup"><span data-stu-id="6d640-142">confidence</span></span>|<span data-ttu-id="6d640-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6d640-143">Int32</span></span>|<span data-ttu-id="6d640-144">Eine ganze Zahl, die die Vertrauenswürdigkeit der Daten innerhalb des Indikators kennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="6d640-144">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="6d640-145">Zulässige Werte sind 0 – 100, wobei 100 der höchste Wert ist.</span><span class="sxs-lookup"><span data-stu-id="6d640-145">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="6d640-146">description</span><span class="sxs-lookup"><span data-stu-id="6d640-146">description</span></span>|<span data-ttu-id="6d640-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d640-147">String</span></span>|<span data-ttu-id="6d640-148">Kurze Beschreibung (100 Zeichen oder kleiner) der Bedrohung, dargestellt durch den Indikator.</span><span class="sxs-lookup"><span data-stu-id="6d640-148">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="6d640-149">diamondModel</span><span class="sxs-lookup"><span data-stu-id="6d640-149">diamondModel</span></span>|<span data-ttu-id="6d640-150">string</span><span class="sxs-lookup"><span data-stu-id="6d640-150">string</span></span>|<span data-ttu-id="6d640-151">Der Bereich des Diamant Modells, in dem dieser Indikator vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="6d640-151">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="6d640-152">Mögliche Werte: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="6d640-152">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="6d640-153">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6d640-153">expirationDateTime</span></span>|<span data-ttu-id="6d640-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d640-154">DateTimeOffset</span></span>| <span data-ttu-id="6d640-155">DateTime-Zeichenfolge, die angibt, wann das Symbol abläuft.</span><span class="sxs-lookup"><span data-stu-id="6d640-155">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="6d640-156">Alle Indikatoren benötigen ein Ablaufdatum, um zu verhindern, dass veraltete Indikatoren im System beibehalten werden.</span><span class="sxs-lookup"><span data-stu-id="6d640-156">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="6d640-157">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="6d640-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d640-158">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6d640-158">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="6d640-159">externalId</span><span class="sxs-lookup"><span data-stu-id="6d640-159">externalId</span></span>|<span data-ttu-id="6d640-160">String</span><span class="sxs-lookup"><span data-stu-id="6d640-160">String</span></span>|<span data-ttu-id="6d640-161">Eine Identifikationsnummer, die den Indikator zurück an das System des Indikator Anbieters bindet (beispielsweise einen Fremdschlüssel).</span><span class="sxs-lookup"><span data-stu-id="6d640-161">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="6d640-162">isActive</span><span class="sxs-lookup"><span data-stu-id="6d640-162">isActive</span></span>|<span data-ttu-id="6d640-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d640-163">Boolean</span></span>|<span data-ttu-id="6d640-164">Wird verwendet, um Indikatoren innerhalb von System zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="6d640-164">Used to deactivate indicators within system.</span></span> <span data-ttu-id="6d640-165">Standardmäßig werden alle übermittelten Indikatoren als aktiv festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6d640-165">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="6d640-166">Anbieter können jedoch vorhandene Indikatoren mit dieser Einstellung auf "false" übermitteln, um Indikatoren im System zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="6d640-166">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="6d640-167">killChain</span><span class="sxs-lookup"><span data-stu-id="6d640-167">killChain</span></span>|<span data-ttu-id="6d640-168">String collection</span><span class="sxs-lookup"><span data-stu-id="6d640-168">String collection</span></span>|<span data-ttu-id="6d640-169">Ein JSON-Array von Zeichenfolgen, die beschreiben, welche Punkte auf der Killkette dieser Indikator erreicht.</span><span class="sxs-lookup"><span data-stu-id="6d640-169">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="6d640-170">Genaue Werte finden Sie weiter unten unter "killChain-Werte".</span><span class="sxs-lookup"><span data-stu-id="6d640-170">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="6d640-171">knownFalsePositives</span><span class="sxs-lookup"><span data-stu-id="6d640-171">knownFalsePositives</span></span>|<span data-ttu-id="6d640-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d640-172">String</span></span>|<span data-ttu-id="6d640-173">Szenarien, in denen das Symbol zu falsch positiven Ergebnissen führen kann.</span><span class="sxs-lookup"><span data-stu-id="6d640-173">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="6d640-174">Dies sollte ein lesbarer Text sein.</span><span class="sxs-lookup"><span data-stu-id="6d640-174">This should be human-readable text.</span></span>|
|<span data-ttu-id="6d640-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d640-175">lastReportedDateTime</span></span>|<span data-ttu-id="6d640-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d640-176">DateTimeOffset</span></span>|<span data-ttu-id="6d640-177">Der Zeitpunkt, zu dem der Indikator zuletzt angezeigt wurde.</span><span class="sxs-lookup"><span data-stu-id="6d640-177">The last time the indicator was seen.</span></span> <span data-ttu-id="6d640-178">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="6d640-178">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d640-179">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="6d640-179">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="6d640-180">malwareFamilyNames</span><span class="sxs-lookup"><span data-stu-id="6d640-180">malwareFamilyNames</span></span>|<span data-ttu-id="6d640-181">String collection</span><span class="sxs-lookup"><span data-stu-id="6d640-181">String collection</span></span>|<span data-ttu-id="6d640-182">Der Name der Schadsoftware-Familie, die mit einem Indikator verknüpft ist, falls vorhanden.</span><span class="sxs-lookup"><span data-stu-id="6d640-182">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="6d640-183">Microsoft bevorzugt den Namen der Microsoft-Schadsoftware-Familie, falls möglich, der über die [Bedrohungs Enzyklopädie](https://www.microsoft.com/wdsi/threats)Windows Defender Security Intelligence gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="6d640-183">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="6d640-184">passiveOnly</span><span class="sxs-lookup"><span data-stu-id="6d640-184">passiveOnly</span></span>|<span data-ttu-id="6d640-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d640-185">Boolean</span></span>|<span data-ttu-id="6d640-186">Bestimmt, ob das Symbol ein Ereignis auslösen soll, das für einen Endbenutzer sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="6d640-186">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="6d640-187">Bei Festlegung auf "true" werden vom Endbenutzer keine Sicherheitstools benachrichtigt, dass ein "Hit" aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="6d640-187">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="6d640-188">Diese wird am häufigsten von Sicherheitsprodukten als Überwachungs-oder Unbeaufsichtigter Modus behandelt, in dem Sie einfach protokollieren, ob eine Übereinstimmung aufgetreten ist, die Aktion jedoch nicht ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="6d640-188">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="6d640-189">Der Standardwert ist "false".</span><span class="sxs-lookup"><span data-stu-id="6d640-189">Default value is false.</span></span>|
|<span data-ttu-id="6d640-190">Schweregrad</span><span class="sxs-lookup"><span data-stu-id="6d640-190">severity</span></span>|<span data-ttu-id="6d640-191">Int32</span><span class="sxs-lookup"><span data-stu-id="6d640-191">Int32</span></span>|<span data-ttu-id="6d640-192">Eine ganze Zahl, die den Schweregrad des böswilligen Verhaltens darstellt, das durch die Daten innerhalb des Indikators identifiziert wird.</span><span class="sxs-lookup"><span data-stu-id="6d640-192">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="6d640-193">Zulässige Werte sind 0 – 5, wobei 5 der schwerste ist und NULL nicht schwerwiegend ist.</span><span class="sxs-lookup"><span data-stu-id="6d640-193">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="6d640-194">Der Standardwert ist 3.</span><span class="sxs-lookup"><span data-stu-id="6d640-194">Default value is 3.</span></span>|
|<span data-ttu-id="6d640-195">tags</span><span class="sxs-lookup"><span data-stu-id="6d640-195">tags</span></span>|<span data-ttu-id="6d640-196">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6d640-196">String collection</span></span>|<span data-ttu-id="6d640-197">Ein JSON-Array von Zeichenfolgen, in dem beliebige Tags/Schlüsselwörter gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="6d640-197">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="6d640-198">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="6d640-198">tlpLevel</span></span>|<span data-ttu-id="6d640-199">string</span><span class="sxs-lookup"><span data-stu-id="6d640-199">string</span></span>| <span data-ttu-id="6d640-200">Ampel-Protokollwert für das Symbol.</span><span class="sxs-lookup"><span data-stu-id="6d640-200">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="6d640-201">Mögliche Werte: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="6d640-201">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="6d640-202">diamondModel-Werte</span><span class="sxs-lookup"><span data-stu-id="6d640-202">diamondModel values</span></span>

<span data-ttu-id="6d640-203">Informationen zu diesem Modell finden Sie unter [Diamond Model](http://diamondmodel.org).</span><span class="sxs-lookup"><span data-stu-id="6d640-203">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="6d640-204">Werte</span><span class="sxs-lookup"><span data-stu-id="6d640-204">Values</span></span> | <span data-ttu-id="6d640-205">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d640-205">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="6d640-206">Gegner</span><span class="sxs-lookup"><span data-stu-id="6d640-206">adversary</span></span>|<span data-ttu-id="6d640-207">Der Indikator beschreibt den Gegner.</span><span class="sxs-lookup"><span data-stu-id="6d640-207">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="6d640-208">Fähigkeit</span><span class="sxs-lookup"><span data-stu-id="6d640-208">capability</span></span>|<span data-ttu-id="6d640-209">Das Symbol ist eine Funktion des Gegners.</span><span class="sxs-lookup"><span data-stu-id="6d640-209">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="6d640-210">Infrastruktur</span><span class="sxs-lookup"><span data-stu-id="6d640-210">infrastructure</span></span>|<span data-ttu-id="6d640-211">Der Indikator beschreibt die Infrastruktur des Gegners.</span><span class="sxs-lookup"><span data-stu-id="6d640-211">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="6d640-212">Opfer</span><span class="sxs-lookup"><span data-stu-id="6d640-212">victim</span></span>|<span data-ttu-id="6d640-213">Der Indikator beschreibt das Opfer des Gegners.</span><span class="sxs-lookup"><span data-stu-id="6d640-213">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="6d640-214">killChain-Werte</span><span class="sxs-lookup"><span data-stu-id="6d640-214">killChain values</span></span>

| <span data-ttu-id="6d640-215">Werte</span><span class="sxs-lookup"><span data-stu-id="6d640-215">Values</span></span> | <span data-ttu-id="6d640-216">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d640-216">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="6d640-217">Aktionen</span><span class="sxs-lookup"><span data-stu-id="6d640-217">Actions</span></span>|<span data-ttu-id="6d640-218">Stellt "Aktionen für Ziele" dar.</span><span class="sxs-lookup"><span data-stu-id="6d640-218">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="6d640-219">Der Angreifer nutzt das kompromittierte System, um Aktionen wie einen verteilten Denial-of-Service-Angriff zu ergreifen.</span><span class="sxs-lookup"><span data-stu-id="6d640-219">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="6d640-220">C2 befindet</span><span class="sxs-lookup"><span data-stu-id="6d640-220">C2</span></span>|<span data-ttu-id="6d640-221">Stellt den Steuerelement Kanal dar, durch den ein kompromittiertes System bearbeitet wird.</span><span class="sxs-lookup"><span data-stu-id="6d640-221">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="6d640-222">Lieferung</span><span class="sxs-lookup"><span data-stu-id="6d640-222">Delivery</span></span>|<span data-ttu-id="6d640-223">Der Prozess der Verteilung des Exploit-Codes auf die Opfer (beispielsweise USB, e-Mail, Websites).</span><span class="sxs-lookup"><span data-stu-id="6d640-223">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="6d640-224">Ausbeutung</span><span class="sxs-lookup"><span data-stu-id="6d640-224">Exploitation</span></span>|<span data-ttu-id="6d640-225">Der Exploitcode nutzt Sicherheitsrisiken aus (beispielsweise Codeausführung).</span><span class="sxs-lookup"><span data-stu-id="6d640-225">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="6d640-226">Installation</span><span class="sxs-lookup"><span data-stu-id="6d640-226">Installation</span></span>|<span data-ttu-id="6d640-227">Installieren von Schadsoftware, nachdem eine Sicherheitsanfälligkeit ausgenutzt wurde.</span><span class="sxs-lookup"><span data-stu-id="6d640-227">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="6d640-228">Aufklärungs</span><span class="sxs-lookup"><span data-stu-id="6d640-228">Reconnaissance</span></span>|<span data-ttu-id="6d640-229">Indikator ist ein Beweis für die Verwendung einer Aktivitätsgruppen-ernteinformationen, die bei zukünftigen Angriffen verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="6d640-229">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="6d640-230">Stationierung</span><span class="sxs-lookup"><span data-stu-id="6d640-230">Weaponization</span></span>|<span data-ttu-id="6d640-231">Aktivieren einer Sicherheitsanfälligkeit in Exploitcode (beispielsweise Schadsoftware).</span><span class="sxs-lookup"><span data-stu-id="6d640-231">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="6d640-232">tlpLevel-Werte</span><span class="sxs-lookup"><span data-stu-id="6d640-232">tlpLevel values</span></span>

<span data-ttu-id="6d640-233">Jeder Indikator muss einen TLP-Wert (Traffic Light Protocol) haben, wenn er übermittelt wird.</span><span class="sxs-lookup"><span data-stu-id="6d640-233">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="6d640-234">Dieser Wert stellt die Vertraulichkeit und den freigabebereich eines bestimmten Indikators dar.</span><span class="sxs-lookup"><span data-stu-id="6d640-234">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="6d640-235">Werte</span><span class="sxs-lookup"><span data-stu-id="6d640-235">Values</span></span> | <span data-ttu-id="6d640-236">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d640-236">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="6d640-237">Weiß</span><span class="sxs-lookup"><span data-stu-id="6d640-237">White</span></span>| <span data-ttu-id="6d640-238">Freigabebereich: unLimited.</span><span class="sxs-lookup"><span data-stu-id="6d640-238">Sharing scope: Unlimited.</span></span> <span data-ttu-id="6d640-239">Indikatoren können frei freigegeben werden, ohne Einschränkungen.</span><span class="sxs-lookup"><span data-stu-id="6d640-239">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="6d640-240">Green</span><span class="sxs-lookup"><span data-stu-id="6d640-240">Green</span></span>| <span data-ttu-id="6d640-241">Freigabebereich: Community.</span><span class="sxs-lookup"><span data-stu-id="6d640-241">Sharing scope: Community.</span></span> <span data-ttu-id="6d640-242">Indikatoren können für die Sicherheitscommunity freigegeben werden.</span><span class="sxs-lookup"><span data-stu-id="6d640-242">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="6d640-243">Bernstein</span><span class="sxs-lookup"><span data-stu-id="6d640-243">Amber</span></span>| <span data-ttu-id="6d640-244">Freigabebereich: Limited.</span><span class="sxs-lookup"><span data-stu-id="6d640-244">Sharing scope: Limited.</span></span> <span data-ttu-id="6d640-245">Dies ist die Standardeinstellung für Indikatoren und schränkt die Freigabe nur für Personen ein, die über einen need-to-Know: 1-Dienst verfügen, und die Dienst Operatoren, die Bedrohungs Intelligenz implementieren. 2) Kunden, deren System (s) Verhalten mit dem Indikator übereinstimmt.</span><span class="sxs-lookup"><span data-stu-id="6d640-245">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="6d640-246">Red</span><span class="sxs-lookup"><span data-stu-id="6d640-246">Red</span></span>| <span data-ttu-id="6d640-247">Freigabebereich: persönlich.</span><span class="sxs-lookup"><span data-stu-id="6d640-247">Sharing scope: Personal.</span></span> <span data-ttu-id="6d640-248">Diese Indikatoren sollen nur direkt und, vorzugsweise persönlich, freigegeben werden.</span><span class="sxs-lookup"><span data-stu-id="6d640-248">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="6d640-249">In der Regel werden TLP-rote Indikatoren aufgrund der vordefinierten Einschränkungen nicht aufgenommen.</span><span class="sxs-lookup"><span data-stu-id="6d640-249">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="6d640-250">Wenn TLP-rote Indikatoren übermittelt \*\*\*\* werden, sollte auch die passiveOnly `True` -Eigenschaft auf festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="6d640-250">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="6d640-251">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d640-251">Response</span></span>

<span data-ttu-id="6d640-252">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d640-252">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="6d640-253">Wenn der optionale Anforderungsheader verwendet wird, gibt die Methode `200 OK` den Antwortcode und das aktualisierte [tiIndicator](../resources/tiIndicator.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6d640-253">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiIndicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d640-254">Beispiele</span><span class="sxs-lookup"><span data-stu-id="6d640-254">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="6d640-255">Beispiel 1: Anforderung ohne vorZugs Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6d640-255">Example 1: Request without Prefer header</span></span>

### <a name="request"></a><span data-ttu-id="6d640-256">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d640-256">Request</span></span>

<span data-ttu-id="6d640-257">Nachfolgend sehen Sie ein Beispiel für die Anforderung ohne `Prefer` den Header.</span><span class="sxs-lookup"><span data-stu-id="6d640-257">The following is an example of the request without the `Prefer` header.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```

### <a name="response"></a><span data-ttu-id="6d640-258">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d640-258">Response</span></span>

<span data-ttu-id="6d640-259">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6d640-259">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="6d640-260">Beispiel 2: Anforderung mit vorZugs Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6d640-260">Example 2: Request with Prefer header</span></span>

### <a name="request"></a><span data-ttu-id="6d640-261">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d640-261">Request</span></span>

<span data-ttu-id="6d640-262">Nachfolgend sehen Sie ein Beispiel für die Anforderung, die `Prefer` den Header enthält.</span><span class="sxs-lookup"><span data-stu-id="6d640-262">The following is an example of the request that includes the `Prefer` header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json
Prefer: return=representation

{
  "additionalInformation": "additionalInformation-after-update",
  "confidence": 42,
  "description": "description-after-update",
}
```

### <a name="response"></a><span data-ttu-id="6d640-263">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d640-263">Response</span></span>

<span data-ttu-id="6d640-264">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6d640-264">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="6d640-265">Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="6d640-265">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6d640-266">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6d640-266">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXXXXXXX",
    "action": null,
    "additionalInformation": "additionalInformation-after-update",
    "activityGroupNames": [],
    "confidence": 42,
    "description": "description-after-update",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
