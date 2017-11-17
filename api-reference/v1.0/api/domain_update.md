# <a name="update-domain"></a><span data-ttu-id="31ae7-101">Domäne aktualisieren</span><span class="sxs-lookup"><span data-stu-id="31ae7-101">Update domain</span></span>

<span data-ttu-id="31ae7-102">Dient zum Aktualisieren der Eigenschaften eines Domänenobjekts.</span><span class="sxs-lookup"><span data-stu-id="31ae7-102">Update the properties of domain object.</span></span>

> <span data-ttu-id="31ae7-103">**Wichtig:** Nur überprüfte Domänen können aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="31ae7-103">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="31ae7-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="31ae7-104">Permissions</span></span>

<span data-ttu-id="31ae7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="31ae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="31ae7-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="31ae7-107">Permission type</span></span>      | <span data-ttu-id="31ae7-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="31ae7-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31ae7-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="31ae7-109">Delegated (work or school account)</span></span> | <span data-ttu-id="31ae7-110">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31ae7-110">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="31ae7-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="31ae7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31ae7-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31ae7-112">Not supported.</span></span>    |
|<span data-ttu-id="31ae7-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="31ae7-113">Application</span></span> | <span data-ttu-id="31ae7-114">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31ae7-114">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31ae7-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="31ae7-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="31ae7-116">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="31ae7-116">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31ae7-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="31ae7-117">Request headers</span></span>

| <span data-ttu-id="31ae7-118">Name</span><span class="sxs-lookup"><span data-stu-id="31ae7-118">Name</span></span>       | <span data-ttu-id="31ae7-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31ae7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="31ae7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="31ae7-120">Authorization</span></span>  | <span data-ttu-id="31ae7-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="31ae7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="31ae7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31ae7-123">Content-Type</span></span>  | <span data-ttu-id="31ae7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="31ae7-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="31ae7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="31ae7-125">Request body</span></span>

<span data-ttu-id="31ae7-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Für optimale Leistung sollten Sie nur geänderte Werte einschließen.</span><span class="sxs-lookup"><span data-stu-id="31ae7-p103">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="31ae7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="31ae7-129">Response</span></span>

<span data-ttu-id="31ae7-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben, aber kein Antworttext.</span><span class="sxs-lookup"><span data-stu-id="31ae7-130">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="31ae7-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="31ae7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31ae7-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31ae7-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/V1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="31ae7-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="31ae7-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->