# <a name="create-section"></a><span data-ttu-id="fd3d1-101">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="fd3d1-101">Create section</span></span>

<span data-ttu-id="fd3d1-102">Mit dieser API können Sie eine neue Ressource des Typs [section](../resources/section.md) in dem angegebenen Notizbuch erstellen.</span><span class="sxs-lookup"><span data-stu-id="fd3d1-102">Create a new [section](../resources/section.md) in the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="fd3d1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd3d1-103">Permissions</span></span>
<span data-ttu-id="fd3d1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd3d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd3d1-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd3d1-106">Permission type</span></span>      | <span data-ttu-id="fd3d1-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd3d1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd3d1-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd3d1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fd3d1-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd3d1-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="fd3d1-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd3d1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd3d1-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd3d1-111">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="fd3d1-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd3d1-112">Application</span></span> | <span data-ttu-id="fd3d1-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd3d1-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd3d1-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd3d1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/sections
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
POST /groups/{id}/onenote/notebooks/{id}/sections
POST /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="fd3d1-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd3d1-115">Request headers</span></span>
| <span data-ttu-id="fd3d1-116">Name</span><span class="sxs-lookup"><span data-stu-id="fd3d1-116">Name</span></span>       | <span data-ttu-id="fd3d1-117">Typ</span><span class="sxs-lookup"><span data-stu-id="fd3d1-117">Type</span></span> | <span data-ttu-id="fd3d1-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd3d1-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fd3d1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd3d1-119">Authorization</span></span>  | <span data-ttu-id="fd3d1-120">string</span><span class="sxs-lookup"><span data-stu-id="fd3d1-120">string</span></span>  | <span data-ttu-id="fd3d1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd3d1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fd3d1-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd3d1-123">Content-Type</span></span> | <span data-ttu-id="fd3d1-124">string</span><span class="sxs-lookup"><span data-stu-id="fd3d1-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="fd3d1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd3d1-125">Request body</span></span>
<span data-ttu-id="fd3d1-126">Geben Sie im Anforderungstext einen Namen für den Abschnitt an.</span><span class="sxs-lookup"><span data-stu-id="fd3d1-126">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="fd3d1-p103">Innerhalb der gleichen Hierarchieebene müssen Abschnittsnamen eindeutig sein. Der Name darf nicht mehr als 50 Zeichen und keines der folgenden Zeichen enthalten: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="fd3d1-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="fd3d1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd3d1-129">Response</span></span>

<span data-ttu-id="fd3d1-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [section](../resources/section.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd3d1-130">If successful, this method returns a `201 Created` response code and a [section](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd3d1-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd3d1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd3d1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd3d1-132">Request</span></span>
<span data-ttu-id="fd3d1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd3d1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_notebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```
##### <a name="response"></a><span data-ttu-id="fd3d1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd3d1-134">Response</span></span>
<span data-ttu-id="fd3d1-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd3d1-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 272

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
