---
title: Warnung aktualisieren
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: efb9911eaeb9d980084c26ef329c7c837c9d04f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815078"
---
# <a name="update-alert"></a><span data-ttu-id="d1383-104">Warnung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d1383-104">Update alert</span></span>

 > <span data-ttu-id="d1383-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d1383-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1383-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1383-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1383-107">Aktualisieren einer bearbeitbaren **Benachrichtigung** -Eigenschaft in eine integrierte Lösung alert Status und Aufgaben in Lösungen synchron.</span><span class="sxs-lookup"><span data-stu-id="d1383-107">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="d1383-108">Dieser Methode wird jede Lösung, die eine Aufzeichnung die Warnung ID wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="d1383-108">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1383-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d1383-109">Permissions</span></span>

<span data-ttu-id="d1383-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1383-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1383-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d1383-112">Permission type</span></span>      | <span data-ttu-id="d1383-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d1383-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1383-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d1383-114">Delegated (work or school account)</span></span> |   <span data-ttu-id="d1383-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1383-115">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="d1383-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d1383-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d1383-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d1383-117">Not supported.</span></span>  |
|<span data-ttu-id="d1383-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d1383-118">Application</span></span> | <span data-ttu-id="d1383-119">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1383-119">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1383-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1383-120">HTTP request</span></span>

> <span data-ttu-id="d1383-121">**Hinweis:** Sie müssen die **Warnung** -ID als Parameter und VendorInformation mit einschließen die `provider` und `vendor` mit dieser Methode.</span><span class="sxs-lookup"><span data-stu-id="d1383-121">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="d1383-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d1383-122">Request headers</span></span>

| <span data-ttu-id="d1383-123">Name</span><span class="sxs-lookup"><span data-stu-id="d1383-123">Name</span></span>       | <span data-ttu-id="d1383-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1383-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d1383-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1383-125">Authorization</span></span>  | <span data-ttu-id="d1383-p105">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1383-p105">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="d1383-128">Prefer</span><span class="sxs-lookup"><span data-stu-id="d1383-128">Prefer</span></span> | <span data-ttu-id="d1383-129">zurückgeben = Darstellung</span><span class="sxs-lookup"><span data-stu-id="d1383-129">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1383-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d1383-130">Request body</span></span>

<span data-ttu-id="d1383-131">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Werte für die entsprechenden Felder, die aktualisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="d1383-131">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d1383-132">Der Textkörper **muss** enthalten die `vendorInformation` -Eigenschaft mit gültigen `provider` und `vendor` Felder.</span><span class="sxs-lookup"><span data-stu-id="d1383-132">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="d1383-133">In der folgenden Tabelle werden die Felder, die für eine Warnung aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="d1383-133">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="d1383-134">Die Werte für vorhandene Eigenschaften, die nicht im Textkörper Anforderung enthalten sind, werden nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="d1383-134">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="d1383-135">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="d1383-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d1383-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1383-136">Property</span></span>   | <span data-ttu-id="d1383-137">Typ</span><span class="sxs-lookup"><span data-stu-id="d1383-137">Type</span></span> |<span data-ttu-id="d1383-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1383-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1383-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="d1383-139">assignedTo</span></span>|<span data-ttu-id="d1383-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1383-140">String</span></span>|<span data-ttu-id="d1383-141">Name des der Analyst die Benachrichtigung wird für die Ursachenanalyse, Untersuchung oder Remediation zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="d1383-141">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="d1383-142">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1383-142">closedDateTime</span></span>|<span data-ttu-id="d1383-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1383-143">DateTimeOffset</span></span>|<span data-ttu-id="d1383-144">Zeitpunkt, an dem die Benachrichtigung geschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="d1383-144">Time at which the alert was closed.</span></span> <span data-ttu-id="d1383-145">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="d1383-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d1383-146">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d1383-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d1383-147">comments</span><span class="sxs-lookup"><span data-stu-id="d1383-147">comments</span></span>|<span data-ttu-id="d1383-148">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="d1383-148">String collection</span></span>|<span data-ttu-id="d1383-149">Analystenkommentare auf die Benachrichtigung (für Kunden alert Management).</span><span class="sxs-lookup"><span data-stu-id="d1383-149">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="d1383-150">Feedback</span><span class="sxs-lookup"><span data-stu-id="d1383-150">feedback</span></span>|<span data-ttu-id="d1383-151">AlertFeedback-Enumeration</span><span class="sxs-lookup"><span data-stu-id="d1383-151">alertFeedback enum</span></span>|<span data-ttu-id="d1383-152">Analyst Feedback auf die Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="d1383-152">Analyst feedback on the alert.</span></span> <span data-ttu-id="d1383-153">Mögliche Werte: sind `unknown`, `truePositive`, `falsePositive` und `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="d1383-153">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="d1383-154">status</span><span class="sxs-lookup"><span data-stu-id="d1383-154">status</span></span>|<span data-ttu-id="d1383-155">AlertStatus-Enumeration</span><span class="sxs-lookup"><span data-stu-id="d1383-155">alertStatus enum</span></span>|<span data-ttu-id="d1383-156">Warnung Lebenszyklusstatus (Phase).</span><span class="sxs-lookup"><span data-stu-id="d1383-156">Alert lifecycle status (stage).</span></span> <span data-ttu-id="d1383-157">Mögliche Werte: sind `unknown`, `newAlert`, `inProgress` und `resolved`.</span><span class="sxs-lookup"><span data-stu-id="d1383-157">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="d1383-158">-Tags hinzugefügtes Markup</span><span class="sxs-lookup"><span data-stu-id="d1383-158">tags</span></span>|<span data-ttu-id="d1383-159">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="d1383-159">String collection</span></span>|<span data-ttu-id="d1383-160">Benutzer definierbare Beschriftungen, die auf eine Warnung angewendet werden können und als filterbedingungen (beispielsweise "HVA", "MAUERN) dienen.</span><span class="sxs-lookup"><span data-stu-id="d1383-160">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="d1383-161">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="d1383-161">vendorInformation</span></span> |[<span data-ttu-id="d1383-162">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="d1383-162">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="d1383-163">Komplexer Typ, das Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider enthält (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="d1383-163">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="d1383-164">**Anbieter und Hersteller Felder sind erforderlich.**</span><span class="sxs-lookup"><span data-stu-id="d1383-164">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="d1383-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1383-165">Response</span></span>

<span data-ttu-id="d1383-166">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1383-166">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="d1383-167">Wenn der optionale Anforderungsheader verwendet wird, gibt die Methode eine `200 OK` Antwortcode und das aktualisierte [Warnung](../resources/alert.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d1383-167">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="d1383-168">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="d1383-168">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="d1383-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1383-169">Request</span></span>

<span data-ttu-id="d1383-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d1383-170">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
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

### <a name="response"></a><span data-ttu-id="d1383-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1383-171">Response</span></span>

<span data-ttu-id="d1383-172">Es folgt ein Beispiel für eine erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="d1383-172">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="d1383-173">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="d1383-173">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="d1383-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1383-174">Request</span></span>

<span data-ttu-id="d1383-175">Das folgende Beispiel zeigt eine Anforderung, die umfasst die `Prefer` Anforderungsheader.</span><span class="sxs-lookup"><span data-stu-id="d1383-175">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
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

### <a name="response"></a><span data-ttu-id="d1383-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1383-176">Response</span></span>

<span data-ttu-id="d1383-177">Im folgenden ist ein Beispiel für die Antwort bei der optionalen `Prefer: return=representation` Anforderungsheader wird verwendet.</span><span class="sxs-lookup"><span data-stu-id="d1383-177">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="d1383-p111">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d1383-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
