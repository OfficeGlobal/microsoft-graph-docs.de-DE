# <a name="domain-verify"></a><span data-ttu-id="9500a-101">domain: verify</span><span class="sxs-lookup"><span data-stu-id="9500a-101">domain: verify</span></span>

<span data-ttu-id="9500a-102">Überprüft den Besitz der Domäne.</span><span class="sxs-lookup"><span data-stu-id="9500a-102">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="9500a-p101">**Wichtig:** Gilt nur für nicht überprüfte Domänen. Bei einer nicht überprüften Domäne hat die Eigenschaft „isVerified“ des [domain](../resources/domain.md)-Objekts den Wert „false“.</span><span class="sxs-lookup"><span data-stu-id="9500a-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="9500a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9500a-105">Permissions</span></span>

<span data-ttu-id="9500a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9500a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="9500a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9500a-108">Permission type</span></span>      | <span data-ttu-id="9500a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9500a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9500a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9500a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9500a-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9500a-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="9500a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9500a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9500a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9500a-113">Not supported.</span></span>    |
|<span data-ttu-id="9500a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9500a-114">Application</span></span> | <span data-ttu-id="9500a-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9500a-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9500a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9500a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="9500a-117">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="9500a-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9500a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9500a-118">Request headers</span></span>

| <span data-ttu-id="9500a-119">Name</span><span class="sxs-lookup"><span data-stu-id="9500a-119">Name</span></span>       | <span data-ttu-id="9500a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9500a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9500a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9500a-121">Authorization</span></span>  | <span data-ttu-id="9500a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9500a-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="9500a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9500a-124">Content-Type</span></span>  | <span data-ttu-id="9500a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9500a-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9500a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9500a-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9500a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9500a-127">Response</span></span>

<span data-ttu-id="9500a-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9500a-128">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9500a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9500a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9500a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9500a-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="9500a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9500a-131">Response</span></span>
<span data-ttu-id="9500a-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9500a-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "name": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->