# <a name="list-sections"></a><span data-ttu-id="ccab2-101">Abschnitte auflisten</span><span class="sxs-lookup"><span data-stu-id="ccab2-101">List sections</span></span>

<span data-ttu-id="ccab2-102">Mit dieser API können Sie eine Liste von Objekten des Typs [section](../resources/section.md) aus der angegebenen Abschnittsgruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="ccab2-102">Retrieve a list of [section](../resources/section.md) objects from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="ccab2-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ccab2-103">Permissions</span></span>
<span data-ttu-id="ccab2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ccab2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ccab2-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ccab2-106">Permission type</span></span>      | <span data-ttu-id="ccab2-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ccab2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccab2-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ccab2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ccab2-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccab2-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ccab2-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ccab2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccab2-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccab2-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ccab2-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ccab2-112">Application</span></span> | <span data-ttu-id="ccab2-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccab2-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccab2-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ccab2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sections
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
GET /groups/{id}/onenote/sectionGroups/{id}/sections
GET /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ccab2-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ccab2-115">Optional query parameters</span></span>
<span data-ttu-id="ccab2-116">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ccab2-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ccab2-117">Die Standardsortierreihenfolge ist `name asc`.</span><span class="sxs-lookup"><span data-stu-id="ccab2-117">The default sort order is `name asc`.</span></span>

<span data-ttu-id="ccab2-p102">Die Standardabfrage erweitert `parentNotebook` und wählt die zugehörigen Eigenschaften `id`, `displayName` und `self` aus. Gültige `expand`-Werte für Abschnitte sind `parentNotebook` und `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="ccab2-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ccab2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ccab2-120">Request headers</span></span>
| <span data-ttu-id="ccab2-121">Name</span><span class="sxs-lookup"><span data-stu-id="ccab2-121">Name</span></span>       | <span data-ttu-id="ccab2-122">Typ</span><span class="sxs-lookup"><span data-stu-id="ccab2-122">Type</span></span> | <span data-ttu-id="ccab2-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ccab2-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ccab2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccab2-124">Authorization</span></span>  | <span data-ttu-id="ccab2-125">string</span><span class="sxs-lookup"><span data-stu-id="ccab2-125">string</span></span>  | <span data-ttu-id="ccab2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ccab2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccab2-128">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ccab2-128">Accept</span></span> | <span data-ttu-id="ccab2-129">string</span><span class="sxs-lookup"><span data-stu-id="ccab2-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ccab2-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ccab2-130">Request body</span></span>
<span data-ttu-id="ccab2-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ccab2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccab2-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ccab2-132">Response</span></span>

<span data-ttu-id="ccab2-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [section](../resources/section.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ccab2-133">If successful, this method returns a `200 OK` response code and a collection of [section](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ccab2-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ccab2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccab2-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ccab2-135">Request</span></span>
<span data-ttu-id="ccab2-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ccab2-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
```
##### <a name="response"></a><span data-ttu-id="ccab2-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="ccab2-137">Response</span></span>
<span data-ttu-id="ccab2-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ccab2-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "isDefault": true,
      "pagesUrl": "pagesUrl-value",
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
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->