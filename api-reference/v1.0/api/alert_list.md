# <a name="list-alerts"></a><span data-ttu-id="e6b11-101">Warnungen auflisten</span><span class="sxs-lookup"><span data-stu-id="e6b11-101">List alerts</span></span>

<span data-ttu-id="e6b11-102">Abrufen einer Liste von [alert](../resources/alert.md)-Objekten.</span><span class="sxs-lookup"><span data-stu-id="e6b11-102">Retrieve a list of nameditem objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6b11-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e6b11-103">Permissions</span></span>

<span data-ttu-id="e6b11-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6b11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e6b11-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e6b11-106">Permission type</span></span>      | <span data-ttu-id="e6b11-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e6b11-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6b11-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e6b11-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="e6b11-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6b11-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="e6b11-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e6b11-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e6b11-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e6b11-111">Not supported.</span></span>  |
|<span data-ttu-id="e6b11-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e6b11-112">Application</span></span> | <span data-ttu-id="e6b11-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6b11-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6b11-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6b11-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6b11-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e6b11-115">Optional query parameters</span></span>

<span data-ttu-id="e6b11-116">Diese Methode unterstützt folgende [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort:</span><span class="sxs-lookup"><span data-stu-id="e6b11-116">This method supports the following [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="e6b11-117">`$top` Gibt die aggregierten Top-Ergebnisse von jedem API-Sicherheits-Anbieter zurück.</span><span class="sxs-lookup"><span data-stu-id="e6b11-117">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="e6b11-118">Um einen alternativen Eigenschaftensatz zurückzugeben, verwenden Sie die OData `$select` Abfrageparameter, um den Satz von Eigenschaften der **Warnungen** anzugeben, den Sie brauchen.</span><span class="sxs-lookup"><span data-stu-id="e6b11-118">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="e6b11-119">Wenn z.B. die Eigenschaften **AssignedTo**, **category**und **severity** zurückgegeben werden sollen, dann fügen Sie die Folgendes für Ihre Abfrage ein: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="e6b11-119">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6b11-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e6b11-120">Request headers</span></span>

| <span data-ttu-id="e6b11-121">Name</span><span class="sxs-lookup"><span data-stu-id="e6b11-121">Name</span></span>      |<span data-ttu-id="e6b11-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6b11-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e6b11-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e6b11-123">Authorization</span></span>  | <span data-ttu-id="e6b11-p103">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e6b11-p103">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6b11-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e6b11-126">Request body</span></span>

<span data-ttu-id="e6b11-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e6b11-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="e6b11-128">Der Anforderungstextkörper wird ignoriert.</span><span class="sxs-lookup"><span data-stu-id="e6b11-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="e6b11-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6b11-129">Response</span></span>

<span data-ttu-id="e6b11-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Sammlung von **alert**-Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e6b11-130">If successful, this method returns a `200 OK` response code and collection of **Attachment** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6b11-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e6b11-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6b11-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e6b11-132">Request</span></span>

<span data-ttu-id="e6b11-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e6b11-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a><span data-ttu-id="e6b11-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e6b11-134">Response</span></span>

<span data-ttu-id="e6b11-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e6b11-135">The following is an example of the response.</span></span>

><span data-ttu-id="e6b11-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="e6b11-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
