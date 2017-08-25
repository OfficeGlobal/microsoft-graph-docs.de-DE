# <a name="enumerate-subsites-of-a-site"></a><span data-ttu-id="c54cf-101">Unterwebsites einer Website aufzählen</span><span class="sxs-lookup"><span data-stu-id="c54cf-101">Enumerate subsites of a site</span></span>

<span data-ttu-id="c54cf-102">Dient zum Abrufen einer Sammlung von Unterwebsites, die für ein [site][]-Objekt definiert sind.</span><span class="sxs-lookup"><span data-stu-id="c54cf-102">Get a collection of subsites defined for a [site][].</span></span>

<span data-ttu-id="c54cf-103">[site]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="c54cf-103">[site]: ../resources/site.md</span></span>

## <a name="permissions"></a><span data-ttu-id="c54cf-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c54cf-104">Permissions</span></span>

<span data-ttu-id="c54cf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c54cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c54cf-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c54cf-107">Permission type</span></span>      | <span data-ttu-id="c54cf-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c54cf-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c54cf-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c54cf-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c54cf-110">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c54cf-110">Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="c54cf-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c54cf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c54cf-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c54cf-112">Not supported.</span></span>    | 
|<span data-ttu-id="c54cf-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c54cf-113">Application</span></span> | <span data-ttu-id="c54cf-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c54cf-114">Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c54cf-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c54cf-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{site-id}/sites
```

## <a name="example"></a><span data-ttu-id="c54cf-116">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c54cf-116">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c54cf-117">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c54cf-117">Request</span></span>

<!-- { "blockType": "request", "name": "list-subsites" } -->

```http
GET /sites/{site-id}/sites
```

#### <a name="response"></a><span data-ttu-id="c54cf-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="c54cf-118">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Enumerate subsites"
} -->
