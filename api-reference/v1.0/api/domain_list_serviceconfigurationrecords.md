# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="593a4-101">serviceConfigurationRecords auflisten</span><span class="sxs-lookup"><span data-stu-id="593a4-101">List serviceConfigurationRecords</span></span>

<span data-ttu-id="593a4-102">Dient zum Abrufen einer Liste von [domainDnsRecord](../resources/domaindnsrecord.md)-Objekten, die erforderlich sind, um Dienste für die Domäne zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="593a4-102">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="593a4-p101">Verwenden Sie die zurückgegebene Liste, um der Zonendatei der Domäne Datensätze hinzufügen. Dies kann über die Domänenregistrierungsstelle oder die Konfiguration des DNS-Servers erfolgen.</span><span class="sxs-lookup"><span data-stu-id="593a4-p101">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="593a4-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="593a4-105">Permissions</span></span>

<span data-ttu-id="593a4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="593a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="593a4-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="593a4-108">Permission type</span></span>      | <span data-ttu-id="593a4-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="593a4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="593a4-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="593a4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="593a4-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="593a4-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="593a4-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="593a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="593a4-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="593a4-113">Not supported.</span></span>    |
|<span data-ttu-id="593a4-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="593a4-114">Application</span></span> | <span data-ttu-id="593a4-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="593a4-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="593a4-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="593a4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="593a4-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="593a4-117">Optional query parameters</span></span>

<span data-ttu-id="593a4-118">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="593a4-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="593a4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="593a4-119">Request headers</span></span>

| <span data-ttu-id="593a4-120">Name</span><span class="sxs-lookup"><span data-stu-id="593a4-120">Name</span></span>      |<span data-ttu-id="593a4-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="593a4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="593a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="593a4-122">Authorization</span></span>  | <span data-ttu-id="593a4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="593a4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="593a4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="593a4-125">Content-Type</span></span>  | <span data-ttu-id="593a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="593a4-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="593a4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="593a4-127">Request body</span></span>

<span data-ttu-id="593a4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="593a4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="593a4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="593a4-129">Response</span></span>

<span data-ttu-id="593a4-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [domainDnsRecord](../resources/domaindnsrecord.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="593a4-130">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="593a4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="593a4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="593a4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="593a4-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="593a4-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="593a4-133">Response</span></span>
<span data-ttu-id="593a4-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="593a4-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedServices": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->