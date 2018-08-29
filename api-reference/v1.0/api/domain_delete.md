# <a name="delete-domain"></a><span data-ttu-id="c1a3c-101">Domäne löschen</span><span class="sxs-lookup"><span data-stu-id="c1a3c-101">Delete domain</span></span>

<span data-ttu-id="c1a3c-102">Dient zum Löschen einer Domäne aus einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-102">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="c1a3c-103">**Wichtig:**</span><span class="sxs-lookup"><span data-stu-id="c1a3c-103">**Important:**</span></span>
> - <span data-ttu-id="c1a3c-104">Gelöschte Domänen können nicht wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-104">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="c1a3c-p101">Bei Löschversuchen tritt ein Fehler auf, wenn noch Ressourcen oder Objekte von der Domäne abhängig sind. Mithilfe der API [domainNameReferences auflisten](domain_list_domainnamereferences.md) können Sie alle abhängige Ressourcen ermitteln.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain_list_domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1a3c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c1a3c-107">Permissions</span></span>

<span data-ttu-id="c1a3c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1a3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="c1a3c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1a3c-110">Permission type</span></span>      | <span data-ttu-id="c1a3c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1a3c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1a3c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1a3c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c1a3c-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c1a3c-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c1a3c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1a3c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1a3c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1a3c-115">Not supported.</span></span>    |
|<span data-ttu-id="c1a3c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1a3c-116">Application</span></span> | <span data-ttu-id="c1a3c-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1a3c-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1a3c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1a3c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="c1a3c-119">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1a3c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1a3c-120">Request headers</span></span>

| <span data-ttu-id="c1a3c-121">Name</span><span class="sxs-lookup"><span data-stu-id="c1a3c-121">Name</span></span>       | <span data-ttu-id="c1a3c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1a3c-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c1a3c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c1a3c-123">Authorization</span></span>  | <span data-ttu-id="c1a3c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1a3c-126">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="c1a3c-126">Content-Type</span></span>  | <span data-ttu-id="c1a3c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c1a3c-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1a3c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1a3c-128">Request body</span></span>

<span data-ttu-id="c1a3c-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1a3c-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1a3c-130">Response</span></span>

<span data-ttu-id="c1a3c-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Es wird keine Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1a3c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1a3c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1a3c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1a3c-134">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="c1a3c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1a3c-135">Response</span></span>

<span data-ttu-id="c1a3c-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1a3c-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->