# <a name="update-alert"></a><span data-ttu-id="76144-101">Warnung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="76144-101">Update alert</span></span>

<span data-ttu-id="76144-102">Aktualisieren einer bearbeitbaren **Benachrichtigung** -Eigenschaft in eine integrierte Lösung alert Status und Aufgaben in Lösungen synchron.</span><span class="sxs-lookup"><span data-stu-id="76144-102">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="76144-103">Dieser Methode wird jede Lösung, die eine Aufzeichnung die Warnung ID wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="76144-103">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="76144-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="76144-104">Permissions</span></span>

<span data-ttu-id="76144-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="76144-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="76144-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="76144-107">Permission type</span></span>      | <span data-ttu-id="76144-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="76144-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76144-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="76144-109">Delegated (work or school account)</span></span> |   <span data-ttu-id="76144-110">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76144-110">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="76144-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="76144-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="76144-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76144-112">Not supported.</span></span>  |
|<span data-ttu-id="76144-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="76144-113">Application</span></span> | <span data-ttu-id="76144-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76144-114">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76144-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="76144-115">HTTP request</span></span>

> <span data-ttu-id="76144-116">**Hinweis:** Sie müssen die **Warnung** -ID als Parameter und VendorInformation mit einschließen die `provider` und `vendor` mit dieser Methode.</span><span class="sxs-lookup"><span data-stu-id="76144-116">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="76144-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="76144-117">Request headers</span></span>

| <span data-ttu-id="76144-118">Name</span><span class="sxs-lookup"><span data-stu-id="76144-118">Name</span></span>       | <span data-ttu-id="76144-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76144-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="76144-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="76144-120">Authorization</span></span>  | <span data-ttu-id="76144-p103">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="76144-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="76144-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="76144-123">Prefer</span></span> | <span data-ttu-id="76144-124">zurückgeben = Darstellung</span><span class="sxs-lookup"><span data-stu-id="76144-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="76144-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="76144-125">Request body</span></span>

<span data-ttu-id="76144-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Werte für die entsprechenden Felder, die aktualisiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="76144-126">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="76144-127">Der Textkörper **muss** enthalten die `vendorInformation` -Eigenschaft mit gültigen `provider` und `vendor` Felder.</span><span class="sxs-lookup"><span data-stu-id="76144-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="76144-128">In der folgenden Tabelle werden die Felder, die für eine Warnung aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="76144-128">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="76144-129">Die Werte für vorhandene Eigenschaften, die nicht im Textkörper Anforderung enthalten sind, werden nicht geändert.</span><span class="sxs-lookup"><span data-stu-id="76144-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="76144-130">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="76144-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="76144-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="76144-131">Property</span></span>   | <span data-ttu-id="76144-132">Typ</span><span class="sxs-lookup"><span data-stu-id="76144-132">Type</span></span> |<span data-ttu-id="76144-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76144-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76144-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="76144-134">assignedTo</span></span>|<span data-ttu-id="76144-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76144-135">String</span></span>|<span data-ttu-id="76144-136">Name des der Analyst die Benachrichtigung wird für die Ursachenanalyse, Untersuchung oder Remediation zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="76144-136">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="76144-137">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="76144-137">closedDateTime</span></span>|<span data-ttu-id="76144-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76144-138">DateTimeOffset</span></span>|<span data-ttu-id="76144-139">Zeitpunkt, an dem die Benachrichtigung geschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="76144-139">Time at which the alert was closed.</span></span> <span data-ttu-id="76144-140">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="76144-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="76144-141">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="76144-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="76144-142">comments</span><span class="sxs-lookup"><span data-stu-id="76144-142">comments</span></span>|<span data-ttu-id="76144-143">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="76144-143">String collection</span></span>|<span data-ttu-id="76144-144">Analystenkommentare auf die Benachrichtigung (für Kunden alert Management).</span><span class="sxs-lookup"><span data-stu-id="76144-144">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="76144-145">Feedback</span><span class="sxs-lookup"><span data-stu-id="76144-145">feedback</span></span>|<span data-ttu-id="76144-146">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="76144-146">alertFeedback</span></span>|<span data-ttu-id="76144-147">Analyst Feedback auf die Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="76144-147">Analyst feedback on the alert.</span></span> <span data-ttu-id="76144-148">Mögliche Werte: sind `unknown`, `truePositive`, `falsePositive` und `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="76144-148">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="76144-149">status</span><span class="sxs-lookup"><span data-stu-id="76144-149">status</span></span>|<span data-ttu-id="76144-150">alertStatus</span><span class="sxs-lookup"><span data-stu-id="76144-150">alertStatus</span></span>|<span data-ttu-id="76144-151">Warnung Lebenszyklusstatus (Phase).</span><span class="sxs-lookup"><span data-stu-id="76144-151">Alert lifecycle status (stage).</span></span> <span data-ttu-id="76144-152">Mögliche Werte: sind `unknown`, `newAlert`, `inProgress` und `resolved`.</span><span class="sxs-lookup"><span data-stu-id="76144-152">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="76144-153">-Tags hinzugefügtes Markup</span><span class="sxs-lookup"><span data-stu-id="76144-153">tags</span></span>|<span data-ttu-id="76144-154">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="76144-154">String collection</span></span>|<span data-ttu-id="76144-155">Benutzer definierbare Beschriftungen, die auf eine Warnung angewendet werden können und als filterbedingungen (beispielsweise "HVA", "MAUERN) dienen.</span><span class="sxs-lookup"><span data-stu-id="76144-155">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="76144-156">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="76144-156">vendorInformation</span></span> |[<span data-ttu-id="76144-157">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="76144-157">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="76144-158">Komplexer Typ, das Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider enthält (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="76144-158">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="76144-159">**Anbieter und Hersteller Felder sind erforderlich.**</span><span class="sxs-lookup"><span data-stu-id="76144-159">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="76144-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="76144-160">Response</span></span>

<span data-ttu-id="76144-161">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76144-161">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="76144-162">Wenn der optionale Anforderungsheader verwendet wird, gibt die Methode eine `200 OK` Antwortcode und das aktualisierte [Warnung](../resources/alert.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="76144-162">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="76144-163">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="76144-163">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="76144-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76144-164">Request</span></span>

<span data-ttu-id="76144-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76144-165">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76144-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="76144-166">Response</span></span>

<span data-ttu-id="76144-167">Es folgt ein Beispiel für eine erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="76144-167">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="76144-168">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="76144-168">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="76144-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76144-169">Request</span></span>

<span data-ttu-id="76144-170">Das folgende Beispiel zeigt eine Anforderung, die umfasst die `Prefer` Anforderungsheader.</span><span class="sxs-lookup"><span data-stu-id="76144-170">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="76144-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="76144-171">Response</span></span>

<span data-ttu-id="76144-172">Im folgenden ist ein Beispiel für die Antwort bei der optionalen `Prefer: return=representation` Anforderungsheader wird verwendet.</span><span class="sxs-lookup"><span data-stu-id="76144-172">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="76144-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="76144-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
