---
title: Warnung aktualisieren
description: Aktualisieren einer bearbeitbaren **Benachrichtigung** -Eigenschaft in eine integrierte Lösung alert Status und Aufgaben in Lösungen synchron. Dieser Methode wird jede Lösung, die eine Aufzeichnung die Warnung ID wurde aktualisiert.
ms.openlocfilehash: 6516d00bc7a542c3aa00244664e08194d96a9640
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019972"
---
# <a name="update-alert"></a><span data-ttu-id="f4ce0-104">Warnung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f4ce0-104">Update alert</span></span>

<span data-ttu-id="f4ce0-105">Aktualisieren einer bearbeitbaren **Benachrichtigung** -Eigenschaft in eine integrierte Lösung alert Status und Aufgaben in Lösungen synchron.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="f4ce0-106">Dieser Methode wird jede Lösung, die eine Aufzeichnung die Warnung ID wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4ce0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f4ce0-107">Permissions</span></span>

<span data-ttu-id="f4ce0-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4ce0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4ce0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f4ce0-110">Permission type</span></span>      | <span data-ttu-id="f4ce0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f4ce0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4ce0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f4ce0-112">Delegated (work or school account)</span></span> |   <span data-ttu-id="f4ce0-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4ce0-113">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="f4ce0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f4ce0-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f4ce0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4ce0-115">Not supported.</span></span>  |
|<span data-ttu-id="f4ce0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f4ce0-116">Application</span></span> | <span data-ttu-id="f4ce0-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4ce0-117">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4ce0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4ce0-118">HTTP request</span></span>

> <span data-ttu-id="f4ce0-119">**Hinweis:** Sie müssen die **Warnung** -ID als Parameter und VendorInformation mit einschließen die `provider` und `vendor` mit dieser Methode.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="f4ce0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f4ce0-120">Request headers</span></span>

| <span data-ttu-id="f4ce0-121">Name</span><span class="sxs-lookup"><span data-stu-id="f4ce0-121">Name</span></span>       | <span data-ttu-id="f4ce0-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4ce0-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f4ce0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4ce0-123">Authorization</span></span>  | <span data-ttu-id="f4ce0-p104">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-p104">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="f4ce0-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="f4ce0-126">Prefer</span></span> | <span data-ttu-id="f4ce0-127">zurückgeben = Darstellung</span><span class="sxs-lookup"><span data-stu-id="f4ce0-127">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4ce0-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f4ce0-128">Request body</span></span>

<span data-ttu-id="f4ce0-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Werte für die entsprechenden Felder, die aktualisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f4ce0-130">Der Textkörper **muss** enthalten die `vendorInformation` -Eigenschaft mit gültigen `provider` und `vendor` Felder.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-130">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="f4ce0-131">In der folgenden Tabelle werden die Felder, die für eine Warnung aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-131">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="f4ce0-132">Die Werte für vorhandene Eigenschaften, die nicht im Textkörper Anforderung enthalten sind, werden nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-132">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="f4ce0-133">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f4ce0-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f4ce0-134">Property</span></span>   | <span data-ttu-id="f4ce0-135">Typ</span><span class="sxs-lookup"><span data-stu-id="f4ce0-135">Type</span></span> |<span data-ttu-id="f4ce0-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4ce0-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4ce0-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="f4ce0-137">assignedTo</span></span>|<span data-ttu-id="f4ce0-138">String</span><span class="sxs-lookup"><span data-stu-id="f4ce0-138">String</span></span>|<span data-ttu-id="f4ce0-139">Name des der Analyst die Benachrichtigung wird für die Ursachenanalyse, Untersuchung oder Remediation zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-139">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="f4ce0-140">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4ce0-140">closedDateTime</span></span>|<span data-ttu-id="f4ce0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4ce0-141">DateTimeOffset</span></span>|<span data-ttu-id="f4ce0-142">Zeitpunkt, an dem die Benachrichtigung geschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-142">Time at which the alert was closed.</span></span> <span data-ttu-id="f4ce0-143">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4ce0-144">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f4ce0-145">comments</span><span class="sxs-lookup"><span data-stu-id="f4ce0-145">comments</span></span>|<span data-ttu-id="f4ce0-146">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f4ce0-146">String collection</span></span>|<span data-ttu-id="f4ce0-147">Analystenkommentare auf die Benachrichtigung (für Kunden alert Management).</span><span class="sxs-lookup"><span data-stu-id="f4ce0-147">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="f4ce0-148">Feedback</span><span class="sxs-lookup"><span data-stu-id="f4ce0-148">feedback</span></span>|<span data-ttu-id="f4ce0-149">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="f4ce0-149">alertFeedback</span></span>|<span data-ttu-id="f4ce0-150">Analyst Feedback auf die Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-150">Analyst feedback on the alert.</span></span> <span data-ttu-id="f4ce0-151">Mögliche Werte: sind `unknown`, `truePositive`, `falsePositive` und `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-151">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="f4ce0-152">status</span><span class="sxs-lookup"><span data-stu-id="f4ce0-152">status</span></span>|<span data-ttu-id="f4ce0-153">alertStatus</span><span class="sxs-lookup"><span data-stu-id="f4ce0-153">alertStatus</span></span>|<span data-ttu-id="f4ce0-154">Warnung Lebenszyklusstatus (Phase).</span><span class="sxs-lookup"><span data-stu-id="f4ce0-154">Alert lifecycle status (stage).</span></span> <span data-ttu-id="f4ce0-155">Mögliche Werte: sind `unknown`, `newAlert`, `inProgress` und `resolved`.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-155">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="f4ce0-156">-Tags hinzugefügtes Markup</span><span class="sxs-lookup"><span data-stu-id="f4ce0-156">tags</span></span>|<span data-ttu-id="f4ce0-157">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f4ce0-157">String collection</span></span>|<span data-ttu-id="f4ce0-158">Benutzer definierbare Beschriftungen, die auf eine Warnung angewendet werden können und als filterbedingungen (beispielsweise "HVA", "MAUERN) dienen.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-158">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="f4ce0-159">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="f4ce0-159">vendorInformation</span></span> |[<span data-ttu-id="f4ce0-160">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="f4ce0-160">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="f4ce0-161">Komplexer Typ, das Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider enthält (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="f4ce0-161">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="f4ce0-162">**Anbieter und Hersteller Felder sind erforderlich.**</span><span class="sxs-lookup"><span data-stu-id="f4ce0-162">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="f4ce0-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4ce0-163">Response</span></span>

<span data-ttu-id="f4ce0-164">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-164">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="f4ce0-165">Wenn der optionale Anforderungsheader verwendet wird, gibt die Methode eine `200 OK` Antwortcode und das aktualisierte [Warnung](../resources/alert.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-165">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="f4ce0-166">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="f4ce0-166">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="f4ce0-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4ce0-167">Request</span></span>

<span data-ttu-id="f4ce0-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-168">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a><span data-ttu-id="f4ce0-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4ce0-169">Response</span></span>

<span data-ttu-id="f4ce0-170">Es folgt ein Beispiel für eine erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-170">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="f4ce0-171">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="f4ce0-171">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="f4ce0-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4ce0-172">Request</span></span>

<span data-ttu-id="f4ce0-173">Das folgende Beispiel zeigt eine Anforderung, die umfasst die `Prefer` Anforderungsheader.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-173">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a><span data-ttu-id="f4ce0-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4ce0-174">Response</span></span>

<span data-ttu-id="f4ce0-175">Im folgenden ist ein Beispiel für die Antwort bei der optionalen `Prefer: return=representation` Anforderungsheader wird verwendet.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-175">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="f4ce0-p110">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f4ce0-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
