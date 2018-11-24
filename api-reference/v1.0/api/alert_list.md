# <a name="list-alerts"></a><span data-ttu-id="9d4e6-101">Warnungen auflisten</span><span class="sxs-lookup"><span data-stu-id="9d4e6-101">List alerts</span></span>

<span data-ttu-id="9d4e6-102">Abrufen einer Liste von [Warnung](../resources/alert.md) -Objekten.</span><span class="sxs-lookup"><span data-stu-id="9d4e6-102">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d4e6-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9d4e6-103">Permissions</span></span>

<span data-ttu-id="9d4e6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d4e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d4e6-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d4e6-106">Permission type</span></span>      | <span data-ttu-id="9d4e6-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d4e6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d4e6-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d4e6-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="9d4e6-109">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d4e6-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="9d4e6-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d4e6-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9d4e6-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d4e6-111">Not supported.</span></span>  |
|<span data-ttu-id="9d4e6-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d4e6-112">Application</span></span> | <span data-ttu-id="9d4e6-113">SecurityEvents.Read.All SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d4e6-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d4e6-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d4e6-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d4e6-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9d4e6-115">Optional query parameters</span></span>

<span data-ttu-id="9d4e6-116">Diese Methode unterstützt die folgenden [Parameter für OData-Abfrage](../../../concepts/query_parameters.md) , mit denen die Antwort anpassen:</span><span class="sxs-lookup"><span data-stu-id="9d4e6-116">This method supports the following [OData query parameters](../../../concepts/query_parameters.md) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="9d4e6-117">`$top`Gibt die aggregierten Top-Ergebnisse aus jeder API Sicherheitsanbieter zurück.</span><span class="sxs-lookup"><span data-stu-id="9d4e6-117">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="9d4e6-118">Um eine alternative Eigenschaftensatz zurückzugeben, verwenden Sie die OData `$select` Abfragen Parameter, um die Gruppe von Eigenschaften der **Benachrichtigung** an, Sie werden soll.</span><span class="sxs-lookup"><span data-stu-id="9d4e6-118">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="9d4e6-119">Wenn **AssignedTo**, **Kategorie**und **Schweregrad** Eigenschaften zurückgeben möchten, fügen Sie beispielsweise die folgenden für Ihre Abfrage: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="9d4e6-119">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d4e6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d4e6-120">Request headers</span></span>

| <span data-ttu-id="9d4e6-121">Name</span><span class="sxs-lookup"><span data-stu-id="9d4e6-121">Name</span></span>      |<span data-ttu-id="9d4e6-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d4e6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d4e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d4e6-123">Authorization</span></span>  | <span data-ttu-id="9d4e6-p103">Bearer {code}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9d4e6-p103">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d4e6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d4e6-126">Request body</span></span>

<span data-ttu-id="9d4e6-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9d4e6-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="9d4e6-128">Textkörper der Anforderung wird ignoriert.</span><span class="sxs-lookup"><span data-stu-id="9d4e6-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="9d4e6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d4e6-129">Response</span></span>

<span data-ttu-id="9d4e6-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext **Benachrichtigung** .</span><span class="sxs-lookup"><span data-stu-id="9d4e6-130">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="9d4e6-131">Wenn ein Statuscode als 2xx oder 404 von einem Anbieter zurückgegeben wird, oder wenn von ein Anbieter Zeitlimit überschritten, die Antwort werden eine `206 Partial Content` Statuscode mit der Antwort Anbieter in der Kopfzeile einer Warnung.</span><span class="sxs-lookup"><span data-stu-id="9d4e6-131">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the providers response in a warning header.</span></span> <span data-ttu-id="9d4e6-132">Weitere Informationen finden Sie unter [Microsoft Graph Security-API-Fehlerantworten](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="9d4e6-132">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="9d4e6-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d4e6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d4e6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d4e6-134">Request</span></span>

<span data-ttu-id="9d4e6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9d4e6-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a><span data-ttu-id="9d4e6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d4e6-136">Response</span></span>

<span data-ttu-id="9d4e6-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9d4e6-137">The following is an example of the response.</span></span>

><span data-ttu-id="9d4e6-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9d4e6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
