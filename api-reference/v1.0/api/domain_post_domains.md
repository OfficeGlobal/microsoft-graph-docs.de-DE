# <a name="create-domain"></a><span data-ttu-id="f4592-101">Domäne erstellen</span><span class="sxs-lookup"><span data-stu-id="f4592-101">Create domain</span></span>

<span data-ttu-id="f4592-102">Fügt eine Domäne zum Mandanten hinzu.</span><span class="sxs-lookup"><span data-stu-id="f4592-102">Adds a domain to the tenant.</span></span>

<span data-ttu-id="f4592-p101">**Wichtig**: Sie können eine zugeordnete Domäne erst dann mit Ihrem Azure AD-Mandanten verwenden, nachdem der Besitz überprüft wurde. Weitere Informationen finden Sie unter [verificationDnsRecords auflisten](domain_list_verificationdnsrecords.md). Stammdomänen erfordern eine Überprüfung. Beispielsweise muss „contoso.com“ überprüft werden. Wenn eine Stammdomäne überprüft wird, werden Unterdomänen der Stammdomäne automatisch überprüft. Beispielsweise wird „subdomain.contoso.com“ automatisch überprüft, wenn „contoso.com“ überprüft wurde.</span><span class="sxs-lookup"><span data-stu-id="f4592-p101">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain_list_verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4592-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f4592-109">Permissions</span></span>

<span data-ttu-id="f4592-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4592-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="f4592-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f4592-112">Permission type</span></span>      | <span data-ttu-id="f4592-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f4592-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4592-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f4592-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f4592-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4592-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f4592-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f4592-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4592-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4592-117">Not supported.</span></span>    |
|<span data-ttu-id="f4592-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f4592-118">Application</span></span> | <span data-ttu-id="f4592-119">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4592-119">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4592-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4592-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="f4592-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f4592-121">Request headers</span></span>
| <span data-ttu-id="f4592-122">Name</span><span class="sxs-lookup"><span data-stu-id="f4592-122">Name</span></span>       | <span data-ttu-id="f4592-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4592-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f4592-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4592-124">Authorization</span></span>  | <span data-ttu-id="f4592-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f4592-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="f4592-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4592-127">Content-Type</span></span>  | <span data-ttu-id="f4592-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f4592-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4592-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f4592-129">Request body</span></span>
<span data-ttu-id="f4592-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [domain](../resources/domain.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f4592-130">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="f4592-p104">Der Anforderungstext enthält die id-Eigenschaft für die neue Domäne. Die id-Eigenschaft ist die einzige Eigenschaft, die angegeben werden kann, und sie ist erforderlich. Der Wert der id-Eigenschaft ist der vollqualifizierte Domänenname, der erstellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="f4592-p104">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="f4592-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4592-134">Response</span></span>

<span data-ttu-id="f4592-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f4592-135">If successful, this method returns `201 Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4592-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f4592-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4592-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4592-137">Request</span></span>

<span data-ttu-id="f4592-138">Geben Sie im Anforderungstext eine JSON-Darstellung des [domain](../resources/domain.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f4592-138">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/V1.0/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a><span data-ttu-id="f4592-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4592-139">Response</span></span>
<span data-ttu-id="f4592-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f4592-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->