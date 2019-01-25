---
title: Warnung aktualisieren
description: Warnung Eigenschaft bearbeitbare in eine integrierte Lösung alert Status und Aufgaben in Lösungen synchron zu aktualisieren.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fc0bc88dad83024d3da2d6f2adf3f16288719cb2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517414"
---
# <a name="update-alert"></a><span data-ttu-id="790ee-103">Warnung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="790ee-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="790ee-104">Aktualisieren einer bearbeitbaren **Benachrichtigung** -Eigenschaft in eine integrierte Lösung alert Status und Aufgaben in Lösungen synchron.</span><span class="sxs-lookup"><span data-stu-id="790ee-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="790ee-105">Dieser Methode wird jede Lösung, die eine Aufzeichnung die Warnung ID wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="790ee-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="790ee-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="790ee-106">Permissions</span></span>

<span data-ttu-id="790ee-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="790ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="790ee-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="790ee-109">Permission type</span></span>      | <span data-ttu-id="790ee-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="790ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="790ee-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="790ee-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="790ee-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="790ee-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="790ee-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="790ee-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="790ee-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="790ee-114">Not supported.</span></span>  |
|<span data-ttu-id="790ee-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="790ee-115">Application</span></span> | <span data-ttu-id="790ee-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="790ee-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="790ee-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="790ee-117">HTTP request</span></span>

> <span data-ttu-id="790ee-118">**Hinweis:** Sie müssen die **Warnung** -ID als Parameter und VendorInformation mit einschließen die `provider` und `vendor` mit dieser Methode.</span><span class="sxs-lookup"><span data-stu-id="790ee-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="790ee-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="790ee-119">Request headers</span></span>

| <span data-ttu-id="790ee-120">Name</span><span class="sxs-lookup"><span data-stu-id="790ee-120">Name</span></span>       | <span data-ttu-id="790ee-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="790ee-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="790ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="790ee-122">Authorization</span></span>  | <span data-ttu-id="790ee-p103">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="790ee-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="790ee-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="790ee-125">Prefer</span></span> | <span data-ttu-id="790ee-126">zurückgeben = Darstellung</span><span class="sxs-lookup"><span data-stu-id="790ee-126">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="790ee-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="790ee-127">Request body</span></span>

<span data-ttu-id="790ee-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Werte für die entsprechenden Felder, die aktualisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="790ee-128">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="790ee-129">Der Textkörper **muss** enthalten die `vendorInformation` -Eigenschaft mit gültigen `provider` und `vendor` Felder.</span><span class="sxs-lookup"><span data-stu-id="790ee-129">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="790ee-130">In der folgenden Tabelle werden die Felder, die für eine Warnung aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="790ee-130">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="790ee-131">Die Werte für vorhandene Eigenschaften, die nicht im Textkörper Anforderung enthalten sind, werden nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="790ee-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="790ee-132">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="790ee-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="790ee-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="790ee-133">Property</span></span>   | <span data-ttu-id="790ee-134">Typ</span><span class="sxs-lookup"><span data-stu-id="790ee-134">Type</span></span> |<span data-ttu-id="790ee-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="790ee-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="790ee-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="790ee-136">assignedTo</span></span>|<span data-ttu-id="790ee-137">String</span><span class="sxs-lookup"><span data-stu-id="790ee-137">String</span></span>|<span data-ttu-id="790ee-138">Name des der Analyst die Benachrichtigung wird für die Ursachenanalyse, Untersuchung oder Remediation zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="790ee-138">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="790ee-139">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="790ee-139">closedDateTime</span></span>|<span data-ttu-id="790ee-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="790ee-140">DateTimeOffset</span></span>|<span data-ttu-id="790ee-141">Zeitpunkt, an dem die Benachrichtigung geschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="790ee-141">Time at which the alert was closed.</span></span> <span data-ttu-id="790ee-142">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="790ee-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="790ee-143">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="790ee-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="790ee-144">comments</span><span class="sxs-lookup"><span data-stu-id="790ee-144">comments</span></span>|<span data-ttu-id="790ee-145">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="790ee-145">String collection</span></span>|<span data-ttu-id="790ee-146">Analystenkommentare auf die Benachrichtigung (für Kunden alert Management).</span><span class="sxs-lookup"><span data-stu-id="790ee-146">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="790ee-147">Feedback</span><span class="sxs-lookup"><span data-stu-id="790ee-147">feedback</span></span>|<span data-ttu-id="790ee-148">AlertFeedback-Enumeration</span><span class="sxs-lookup"><span data-stu-id="790ee-148">alertFeedback enum</span></span>|<span data-ttu-id="790ee-149">Analyst Feedback auf die Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="790ee-149">Analyst feedback on the alert.</span></span> <span data-ttu-id="790ee-150">Mögliche Werte: sind `unknown`, `truePositive`, `falsePositive` und `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="790ee-150">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="790ee-151">status</span><span class="sxs-lookup"><span data-stu-id="790ee-151">status</span></span>|<span data-ttu-id="790ee-152">AlertStatus-Enumeration</span><span class="sxs-lookup"><span data-stu-id="790ee-152">alertStatus enum</span></span>|<span data-ttu-id="790ee-153">Warnung Lebenszyklusstatus (Phase).</span><span class="sxs-lookup"><span data-stu-id="790ee-153">Alert lifecycle status (stage).</span></span> <span data-ttu-id="790ee-154">Mögliche Werte: sind `unknown`, `newAlert`, `inProgress` und `resolved`.</span><span class="sxs-lookup"><span data-stu-id="790ee-154">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="790ee-155">tags</span><span class="sxs-lookup"><span data-stu-id="790ee-155">tags</span></span>|<span data-ttu-id="790ee-156">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="790ee-156">String collection</span></span>|<span data-ttu-id="790ee-157">Benutzer definierbare Beschriftungen, die auf eine Warnung angewendet werden können und als filterbedingungen (beispielsweise "HVA", "MAUERN) dienen.</span><span class="sxs-lookup"><span data-stu-id="790ee-157">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="790ee-158">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="790ee-158">vendorInformation</span></span> |[<span data-ttu-id="790ee-159">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="790ee-159">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="790ee-160">Komplexer Typ, das Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider enthält (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="790ee-160">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="790ee-161">**Anbieter und Hersteller Felder sind erforderlich.**</span><span class="sxs-lookup"><span data-stu-id="790ee-161">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="790ee-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="790ee-162">Response</span></span>

<span data-ttu-id="790ee-163">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="790ee-163">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="790ee-164">Wenn der optionale Anforderungsheader verwendet wird, gibt die Methode eine `200 OK` Antwortcode und das aktualisierte [Warnung](../resources/alert.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="790ee-164">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="790ee-165">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="790ee-165">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="790ee-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="790ee-166">Request</span></span>

<span data-ttu-id="790ee-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="790ee-167">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="790ee-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="790ee-168">Response</span></span>

<span data-ttu-id="790ee-169">Es folgt ein Beispiel für eine erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="790ee-169">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="790ee-170">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="790ee-170">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="790ee-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="790ee-171">Request</span></span>

<span data-ttu-id="790ee-172">Das folgende Beispiel zeigt eine Anforderung, die umfasst die `Prefer` Anforderungsheader.</span><span class="sxs-lookup"><span data-stu-id="790ee-172">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="790ee-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="790ee-173">Response</span></span>

<span data-ttu-id="790ee-174">Im folgenden ist ein Beispiel für die Antwort bei der optionalen `Prefer: return=representation` Anforderungsheader wird verwendet.</span><span class="sxs-lookup"><span data-stu-id="790ee-174">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="790ee-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="790ee-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
