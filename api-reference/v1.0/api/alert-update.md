---
title: Warnung aktualisieren
description: Aktualisieren einer bearbeitbaren **Benachrichtigung** -Eigenschaft in eine integrierte Lösung alert Status und Aufgaben in Lösungen synchron. Dieser Methode wird jede Lösung, die eine Aufzeichnung die Warnung ID wurde aktualisiert.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 42bc945dde726466439802350796d628ee438e22
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967319"
---
# <a name="update-alert"></a><span data-ttu-id="b5b07-104">Warnung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b5b07-104">Update alert</span></span>

<span data-ttu-id="b5b07-105">Aktualisieren einer bearbeitbaren **Benachrichtigung** -Eigenschaft in eine integrierte Lösung alert Status und Aufgaben in Lösungen synchron.</span><span class="sxs-lookup"><span data-stu-id="b5b07-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="b5b07-106">Dieser Methode wird jede Lösung, die eine Aufzeichnung die Warnung ID wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="b5b07-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5b07-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b5b07-107">Permissions</span></span>

<span data-ttu-id="b5b07-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5b07-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5b07-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5b07-110">Permission type</span></span>                        | <span data-ttu-id="b5b07-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5b07-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="b5b07-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5b07-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5b07-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5b07-113">SecurityEvents.ReadWrite.All</span></span>        |
| <span data-ttu-id="b5b07-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5b07-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5b07-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5b07-115">Not supported.</span></span>                      |
| <span data-ttu-id="b5b07-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5b07-116">Application</span></span>                            | <span data-ttu-id="b5b07-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5b07-117">SecurityEvents.ReadWrite.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="b5b07-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5b07-118">HTTP request</span></span>

> <span data-ttu-id="b5b07-119">**Hinweis:** Sie müssen die **Warnung** -ID als Parameter und VendorInformation mit einschließen die `provider` und `vendor` mit dieser Methode.</span><span class="sxs-lookup"><span data-stu-id="b5b07-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="b5b07-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5b07-120">Request headers</span></span>

| <span data-ttu-id="b5b07-121">Name</span><span class="sxs-lookup"><span data-stu-id="b5b07-121">Name</span></span>          | <span data-ttu-id="b5b07-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5b07-122">Description</span></span>              |
|:--------------|:-------------------------|
| <span data-ttu-id="b5b07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5b07-123">Authorization</span></span> | <span data-ttu-id="b5b07-p104">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b5b07-p104">Bearer {code}. Required.</span></span> |
| <span data-ttu-id="b5b07-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="b5b07-126">Prefer</span></span>        | <span data-ttu-id="b5b07-127">zurückgeben = Darstellung</span><span class="sxs-lookup"><span data-stu-id="b5b07-127">return=representation</span></span>    |

## <a name="request-body"></a><span data-ttu-id="b5b07-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5b07-128">Request body</span></span>

<span data-ttu-id="b5b07-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Werte für die entsprechenden Felder, die aktualisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="b5b07-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b5b07-130">Der Textkörper **muss** enthalten die `vendorInformation` -Eigenschaft mit gültigen `provider` und `vendor` Felder.</span><span class="sxs-lookup"><span data-stu-id="b5b07-130">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="b5b07-131">In der folgenden Tabelle werden die Felder, die für eine Warnung aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="b5b07-131">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="b5b07-132">Die Werte für vorhandene Eigenschaften, die nicht im Textkörper Anforderung enthalten sind, werden nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="b5b07-132">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="b5b07-133">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="b5b07-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b5b07-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5b07-134">Property</span></span>          | <span data-ttu-id="b5b07-135">Typ</span><span class="sxs-lookup"><span data-stu-id="b5b07-135">Type</span></span>                                                                   | <span data-ttu-id="b5b07-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5b07-136">Description</span></span> |
|:------------------|:-----------------------------------------------------------------------|:--|
| <span data-ttu-id="b5b07-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="b5b07-137">assignedTo</span></span>        | <span data-ttu-id="b5b07-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5b07-138">String</span></span>                                                                 | <span data-ttu-id="b5b07-139">Name des der Analyst die Benachrichtigung wird für die Ursachenanalyse, Untersuchung oder Remediation zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="b5b07-139">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span> |
| <span data-ttu-id="b5b07-140">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5b07-140">closedDateTime</span></span>    | <span data-ttu-id="b5b07-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5b07-141">DateTimeOffset</span></span>                                                         | <span data-ttu-id="b5b07-142">Zeitpunkt, an dem die Benachrichtigung geschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="b5b07-142">Time at which the alert was closed.</span></span> <span data-ttu-id="b5b07-143">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="b5b07-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b5b07-144">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b5b07-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="b5b07-145">comments</span><span class="sxs-lookup"><span data-stu-id="b5b07-145">comments</span></span>          | <span data-ttu-id="b5b07-146">String collection</span><span class="sxs-lookup"><span data-stu-id="b5b07-146">String collection</span></span>                                                      | <span data-ttu-id="b5b07-147">Analystenkommentare auf die Benachrichtigung (für Kunden alert Management).</span><span class="sxs-lookup"><span data-stu-id="b5b07-147">Analyst comments on the alert (for customer alert management).</span></span> |
| <span data-ttu-id="b5b07-148">Feedback</span><span class="sxs-lookup"><span data-stu-id="b5b07-148">feedback</span></span>          | <span data-ttu-id="b5b07-149">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="b5b07-149">alertFeedback</span></span>                                                          | <span data-ttu-id="b5b07-150">Analyst Feedback auf die Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="b5b07-150">Analyst feedback on the alert.</span></span> <span data-ttu-id="b5b07-151">Mögliche Werte: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="b5b07-151">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span> |
| <span data-ttu-id="b5b07-152">status</span><span class="sxs-lookup"><span data-stu-id="b5b07-152">status</span></span>            | <span data-ttu-id="b5b07-153">alertStatus</span><span class="sxs-lookup"><span data-stu-id="b5b07-153">alertStatus</span></span>                                                            | <span data-ttu-id="b5b07-154">Warnung Lebenszyklus-Status (Phase).</span><span class="sxs-lookup"><span data-stu-id="b5b07-154">Alert life cycle status (stage).</span></span> <span data-ttu-id="b5b07-155">Mögliche Werte: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="b5b07-155">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span> |
| <span data-ttu-id="b5b07-156">tags</span><span class="sxs-lookup"><span data-stu-id="b5b07-156">tags</span></span>              | <span data-ttu-id="b5b07-157">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b5b07-157">String collection</span></span>                                                      | <span data-ttu-id="b5b07-158">Benutzer definierbare Beschriftungen, die auf eine Warnung angewendet werden können und als filterbedingungen (beispielsweise "HVA", "MAUERN) dienen.</span><span class="sxs-lookup"><span data-stu-id="b5b07-158">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span> |
| <span data-ttu-id="b5b07-159">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="b5b07-159">vendorInformation</span></span> | [<span data-ttu-id="b5b07-160">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="b5b07-160">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="b5b07-161">Komplexer Typ, das Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider enthält (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="b5b07-161">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="b5b07-162">**Anbieter und Hersteller Felder sind erforderlich.**</span><span class="sxs-lookup"><span data-stu-id="b5b07-162">**Provider and vendor fields are required.**</span></span> |

## <a name="response"></a><span data-ttu-id="b5b07-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5b07-163">Response</span></span>

<span data-ttu-id="b5b07-164">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5b07-164">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="b5b07-165">Wenn der optionale Anforderungsheader verwendet wird, gibt die Methode eine `200 OK` Antwortcode und das aktualisierte [Warnung](../resources/alert.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b5b07-165">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5b07-166">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b5b07-166">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="b5b07-167">In Beispiel 1: Anforderung ohne bevorzugen-header</span><span class="sxs-lookup"><span data-stu-id="b5b07-167">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="b5b07-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5b07-168">Request</span></span>

<span data-ttu-id="b5b07-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5b07-169">The following is an example of the request.</span></span>
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
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="b5b07-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5b07-170">Response</span></span>

<span data-ttu-id="b5b07-171">Es folgt ein Beispiel für eine erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="b5b07-171">The following is an example of a successful response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="b5b07-172">Beispiel 2: Anforderung mit bevorzugen-header</span><span class="sxs-lookup"><span data-stu-id="b5b07-172">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="b5b07-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5b07-173">Request</span></span>

<span data-ttu-id="b5b07-174">Das folgende Beispiel zeigt eine Anforderung, die umfasst die `Prefer` Anforderungsheader.</span><span class="sxs-lookup"><span data-stu-id="b5b07-174">The following example shows a request that includes the `Prefer` request header.</span></span>

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
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```

#### <a name="response"></a><span data-ttu-id="b5b07-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5b07-175">Response</span></span>

<span data-ttu-id="b5b07-176">Im folgenden ist ein Beispiel für die Antwort bei der optionalen `Prefer: return=representation` Anforderungsheader wird verwendet.</span><span class="sxs-lookup"><span data-stu-id="b5b07-176">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="b5b07-p110">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b5b07-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
