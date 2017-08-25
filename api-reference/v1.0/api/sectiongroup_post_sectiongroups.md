# <a name="create-sectiongroup"></a><span data-ttu-id="cafea-101">sectionGroup erstellen</span><span class="sxs-lookup"><span data-stu-id="cafea-101">Create sectionGroup</span></span>

<span data-ttu-id="cafea-102">Mit dieser API können Sie eine neue [Abschnittsgruppe](../resources/sectiongroup.md) in der angegebenen Abschnittsgruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="cafea-102">Create a new [section group](../resources/sectiongroup.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="cafea-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cafea-103">Permissions</span></span>
<span data-ttu-id="cafea-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cafea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cafea-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cafea-106">Permission type</span></span>      | <span data-ttu-id="cafea-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cafea-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="cafea-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cafea-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cafea-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cafea-109">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="cafea-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cafea-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cafea-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cafea-111">Notes.Create, Notes.ReadWrite, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="cafea-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cafea-112">Application</span></span> | <span data-ttu-id="cafea-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cafea-113">Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cafea-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cafea-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sectionGroups
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
POST /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
POST /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="request-headers"></a><span data-ttu-id="cafea-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cafea-115">Request headers</span></span>
| <span data-ttu-id="cafea-116">Name</span><span class="sxs-lookup"><span data-stu-id="cafea-116">Name</span></span>       | <span data-ttu-id="cafea-117">Typ</span><span class="sxs-lookup"><span data-stu-id="cafea-117">Type</span></span> | <span data-ttu-id="cafea-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cafea-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cafea-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="cafea-119">Authorization</span></span>  | <span data-ttu-id="cafea-120">string</span><span class="sxs-lookup"><span data-stu-id="cafea-120">string</span></span>  | <span data-ttu-id="cafea-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cafea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cafea-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cafea-123">Content-Type</span></span> | <span data-ttu-id="cafea-124">string</span><span class="sxs-lookup"><span data-stu-id="cafea-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="cafea-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cafea-125">Request body</span></span>
<span data-ttu-id="cafea-126">Geben Sie im Anforderungstext einen Namen für die Abschnittsgruppe an.</span><span class="sxs-lookup"><span data-stu-id="cafea-126">In the request body, supply a name for the section group.</span></span>

<span data-ttu-id="cafea-p103">Innerhalb der gleichen Hierarchieebene müssen Abschnittsgruppennamen eindeutig sein. Der Name darf nicht mehr als 50 Zeichen und keines der folgenden Zeichen enthalten: ?*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="cafea-p103">Within the same hierarchy level, section group names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="cafea-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cafea-129">Response</span></span>

<span data-ttu-id="cafea-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [sectionGroup](../resources/sectiongroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cafea-130">If successful, this method returns a `201 Created` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cafea-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cafea-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cafea-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cafea-132">Request</span></span>
<span data-ttu-id="cafea-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cafea-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_sectiongroup_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
Content-type: application/json
Content-length: 30

{
  "displayName": "Section group name"
}
```
##### <a name="response"></a><span data-ttu-id="cafea-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cafea-134">Response</span></span>
<span data-ttu-id="cafea-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cafea-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

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
  "lastModifiedBy": 
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create SectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->