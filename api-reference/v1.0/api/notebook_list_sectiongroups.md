# <a name="list-sectiongroups"></a><span data-ttu-id="cacd1-101">sectionGroups auflisten</span><span class="sxs-lookup"><span data-stu-id="cacd1-101">List sectionGroups</span></span>

<span data-ttu-id="cacd1-102">Mit dieser API können Sie eine Liste von [Abschnittsgruppen](../resources/sectiongroup.md) aus dem angegebenen Notizbuch abrufen.</span><span class="sxs-lookup"><span data-stu-id="cacd1-102">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="cacd1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cacd1-103">Permissions</span></span>
<span data-ttu-id="cacd1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cacd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cacd1-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cacd1-106">Permission type</span></span>      | <span data-ttu-id="cacd1-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cacd1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cacd1-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cacd1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cacd1-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cacd1-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="cacd1-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cacd1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cacd1-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cacd1-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="cacd1-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cacd1-112">Application</span></span> | <span data-ttu-id="cacd1-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cacd1-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cacd1-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cacd1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sectionGroups
GET /groups/{id}/onenote/notebooks/{id}/sectionGroups
GET /sites/{id}/onenote/notebooks/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cacd1-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cacd1-115">Optional query parameters</span></span>
<span data-ttu-id="cacd1-116">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cacd1-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="cacd1-117">Die Standardsortierreihenfolge ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="cacd1-117">The default sort order is `name asc`.</span></span>

<span data-ttu-id="cacd1-p102">Die Standardabfrage erweitert `parentNotebook` und wählt die zugehörigen Eigenschaften `id`, `displayName` und `self` aus. Gültige `expand`-Werte für Abschnittsgruppen sind `sections`, `sectionGroups`, `parentNotebook` und `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="cacd1-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cacd1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cacd1-120">Request headers</span></span>
| <span data-ttu-id="cacd1-121">Name</span><span class="sxs-lookup"><span data-stu-id="cacd1-121">Name</span></span>       | <span data-ttu-id="cacd1-122">Typ</span><span class="sxs-lookup"><span data-stu-id="cacd1-122">Type</span></span> | <span data-ttu-id="cacd1-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cacd1-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cacd1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cacd1-124">Authorization</span></span>  | <span data-ttu-id="cacd1-125">string</span><span class="sxs-lookup"><span data-stu-id="cacd1-125">string</span></span>  | <span data-ttu-id="cacd1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cacd1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cacd1-128">Accept</span><span class="sxs-lookup"><span data-stu-id="cacd1-128">Accept</span></span> | <span data-ttu-id="cacd1-129">string</span><span class="sxs-lookup"><span data-stu-id="cacd1-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="cacd1-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cacd1-130">Request body</span></span>
<span data-ttu-id="cacd1-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cacd1-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cacd1-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="cacd1-132">Response</span></span>

<span data-ttu-id="cacd1-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [sectionGroup](../resources/sectiongroup.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cacd1-133">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cacd1-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cacd1-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cacd1-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cacd1-135">Request</span></span>
<span data-ttu-id="cacd1-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cacd1-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="cacd1-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="cacd1-137">Response</span></span>
<span data-ttu-id="cacd1-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cacd1-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
    {
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "displayName": "name-value",
      "createdBy": {
        "user": {
          "id": "id-value",
          "displayName": "displayName-value"
        }
      },
      "lastModifiedBy": {
        "user": {
          "id": "id-value",
          "displayName": "displayName-value"
        }
       }
     }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
