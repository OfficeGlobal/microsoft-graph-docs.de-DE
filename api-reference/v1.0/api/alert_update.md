# <a name="update-alert"></a><span data-ttu-id="0eff5-101">Update-Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="0eff5-101">Update alert</span></span>

<span data-ttu-id="0eff5-102">Aktualisieren Sie eine editierbare **alert**-Eigenschaft innerhalb einer integrierten Lösung, um den Benachrichtigungsstatus und die Zuweisungen zwischen den Lösungen synchron zu halten.</span><span class="sxs-lookup"><span data-stu-id="0eff5-102">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="0eff5-103">Diese Methode aktualisiert jede Lösung, die einen Datensatz der referenzierten alert-ID hat.</span><span class="sxs-lookup"><span data-stu-id="0eff5-103">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="0eff5-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0eff5-104">Permissions</span></span>

<span data-ttu-id="0eff5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0eff5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0eff5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0eff5-107">Permission type</span></span>      | <span data-ttu-id="0eff5-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0eff5-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0eff5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0eff5-109">Delegated (work or school account)</span></span> |   <span data-ttu-id="0eff5-110">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eff5-110">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="0eff5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0eff5-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0eff5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0eff5-112">Not supported.</span></span>  |
|<span data-ttu-id="0eff5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0eff5-113">Application</span></span> | <span data-ttu-id="0eff5-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eff5-114">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0eff5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0eff5-115">HTTP request</span></span>

> <span data-ttu-id="0eff5-116">**Hinweis:** Bei dieser Methode müssen Sie die **alert** ID als Parameter und „vendorInformation” mit der `provider` und `vendor` angeben.</span><span class="sxs-lookup"><span data-stu-id="0eff5-116">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="0eff5-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0eff5-117">Request headers</span></span>

| <span data-ttu-id="0eff5-118">Name</span><span class="sxs-lookup"><span data-stu-id="0eff5-118">Name</span></span>       | <span data-ttu-id="0eff5-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0eff5-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0eff5-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0eff5-120">Authorization</span></span>  | <span data-ttu-id="0eff5-p103">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0eff5-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="0eff5-123">Bevorzugt</span><span class="sxs-lookup"><span data-stu-id="0eff5-123">Prefer</span></span> | <span data-ttu-id="0eff5-124">zurückgeben = Darstellung</span><span class="sxs-lookup"><span data-stu-id="0eff5-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="0eff5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0eff5-125">Request body</span></span>

<span data-ttu-id="0eff5-126">Geben Sie im Request-Body eine JSON-Darstellung der Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0eff5-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0eff5-127">Der Body **muss** die `vendorInformation` Eigenschaft mit gültigen `provider` und `vendor` Feldern enthalten.</span><span class="sxs-lookup"><span data-stu-id="0eff5-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="0eff5-128">Die folgende Tabelle listet die Felder auf, die für eine Benachrichtigung aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="0eff5-128">The following table lists the authentication settings that can be changed for an authentication provider.</span></span> <span data-ttu-id="0eff5-129">Die Werte für bestehende Eigenschaften, die nicht im Body des Requests enthalten sind, ändern sich nicht.</span><span class="sxs-lookup"><span data-stu-id="0eff5-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="0eff5-130">Um die beste Leistung zu erzielen, sollten Sie keine vorhandenen Werte einbeziehen, die sich nicht geändert haben.</span><span class="sxs-lookup"><span data-stu-id="0eff5-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0eff5-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0eff5-131">Property</span></span>   | <span data-ttu-id="0eff5-132">Typ</span><span class="sxs-lookup"><span data-stu-id="0eff5-132">Type</span></span> |<span data-ttu-id="0eff5-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0eff5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0eff5-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="0eff5-134">assignedTo</span></span>|<span data-ttu-id="0eff5-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0eff5-135">String</span></span>|<span data-ttu-id="0eff5-136">Name des Analysten, dem die Benachrichtigung für die Selektierung, Untersuchung oder Wartung zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="0eff5-136">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="0eff5-137">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="0eff5-137">closedDateTime</span></span>|<span data-ttu-id="0eff5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0eff5-138">DateTimeOffset</span></span>|<span data-ttu-id="0eff5-139">Zeitpunkt, an dem die Benachrichtigung geschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="0eff5-139">Time at which the alert was closed.</span></span> <span data-ttu-id="0eff5-140">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="0eff5-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0eff5-141">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0eff5-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="0eff5-142">comments</span><span class="sxs-lookup"><span data-stu-id="0eff5-142">comments</span></span>|<span data-ttu-id="0eff5-143">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0eff5-143">String collection</span></span>|<span data-ttu-id="0eff5-144">Analystenkommentare auf die Benachrichtigung (für Kunden- Benachrichtigungsmanagement).</span><span class="sxs-lookup"><span data-stu-id="0eff5-144">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="0eff5-145">Rückmeldung</span><span class="sxs-lookup"><span data-stu-id="0eff5-145">Feedback</span></span>|<span data-ttu-id="0eff5-146">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="0eff5-146">alertFeedback</span></span>|<span data-ttu-id="0eff5-147">Analysten-Feedback auf die Benachrichtigung.</span><span class="sxs-lookup"><span data-stu-id="0eff5-147">Analyst feedback on the alert.</span></span> <span data-ttu-id="0eff5-148">Mögliche Werte: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="0eff5-148">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="0eff5-149">Status</span><span class="sxs-lookup"><span data-stu-id="0eff5-149">status</span></span>|<span data-ttu-id="0eff5-150">alertStatus</span><span class="sxs-lookup"><span data-stu-id="0eff5-150">alertStatus</span></span>|<span data-ttu-id="0eff5-151">Benachrichtigungs-Lebenszyklusstatus (Phase).</span><span class="sxs-lookup"><span data-stu-id="0eff5-151">Alert lifecycle status (stage).</span></span> <span data-ttu-id="0eff5-152">Mögliche Werte: `unknown`, `newAlert`, `inProgress`, `resolved`.</span><span class="sxs-lookup"><span data-stu-id="0eff5-152">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="0eff5-153">tags</span><span class="sxs-lookup"><span data-stu-id="0eff5-153">tags</span></span>|<span data-ttu-id="0eff5-154">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0eff5-154">String collection</span></span>|<span data-ttu-id="0eff5-155">Benutzerdefinierbare Labels, die auf eine Benachrichtigung angewendet werden können und als Filterbedingungen dienen können (z.B. "HVA", "SAW").</span><span class="sxs-lookup"><span data-stu-id="0eff5-155">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="0eff5-156">vendorInformation \*</span><span class="sxs-lookup"><span data-stu-id="0eff5-156">vendorInformation \*</span></span>|[<span data-ttu-id="0eff5-157">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="0eff5-157">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="0eff5-158">Komplexer Typ, der Angaben zum Sicherheitsprodukt/Dienstleister, Anbieter und Unteranbieter enthält (z. B. Lieferant=Microsoft; Anbieter=Windows Defender ATP; Unteranbieter=AppLocker).</span><span class="sxs-lookup"><span data-stu-id="0eff5-158">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="0eff5-159">**Die Felder Anbieter und Lieferant sind Pflichtfelder.**</span><span class="sxs-lookup"><span data-stu-id="0eff5-159">**Provider and vendor fields are required.**</span></span>|
<span data-ttu-id="0eff5-160">(\* Kennzeichnet ein Pflichtfeld.)</span><span class="sxs-lookup"><span data-stu-id="0eff5-160">(\* Indicates a mandatory field.)</span></span>

## <a name="response"></a><span data-ttu-id="0eff5-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="0eff5-161">Response</span></span>

<span data-ttu-id="0eff5-162">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0eff5-162">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="0eff5-163">Wird der optionale Anforderungsheader verwendet, gibt die Methode einen `200 OK` Antwortcode und das aktualisierte [alert](../resources/alert.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0eff5-163">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="0eff5-164">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="0eff5-164">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="0eff5-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0eff5-165">Request</span></span>

<span data-ttu-id="0eff5-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0eff5-166">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0eff5-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="0eff5-167">Response</span></span>

<span data-ttu-id="0eff5-168">Es folgt ein Beispiel für die erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="0eff5-168">The following is an example of a response to a  event.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="0eff5-169">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="0eff5-169">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="0eff5-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0eff5-170">Request</span></span>

<span data-ttu-id="0eff5-171">Das folgende Beispiel zeigt eine Anforderung, die den `Prefer` Anforderungsheader enthält.</span><span class="sxs-lookup"><span data-stu-id="0eff5-171">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="0eff5-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="0eff5-172">Response</span></span>

<span data-ttu-id="0eff5-173">Das folgende Beispiel zeigt die Antwort, wenn der optionale `Prefer: return=representation` Anforderungsheader verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0eff5-173">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="0eff5-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Alle Eigenschaften werden von einem aktuellen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0eff5-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
