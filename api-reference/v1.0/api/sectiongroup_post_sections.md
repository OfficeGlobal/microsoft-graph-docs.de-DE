# <a name="create-section"></a><span data-ttu-id="86083-101">Abschnitt erstellen</span><span class="sxs-lookup"><span data-stu-id="86083-101">Create section</span></span>

<span data-ttu-id="86083-102">Mit dieser API können Sie eine neue Ressource des Typs [onenoteSection](../resources/section.md) in der angegebenen Abschnittsgruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="86083-102">Create a new [section](../resources/section.md) in the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="86083-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="86083-103">Permissions</span></span>
<span data-ttu-id="86083-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="86083-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="86083-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86083-106">Permission type</span></span>      | <span data-ttu-id="86083-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86083-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86083-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86083-108">Delegated (work or school account)</span></span> | <span data-ttu-id="86083-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86083-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="86083-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86083-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86083-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86083-111">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="86083-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86083-112">Application</span></span> | <span data-ttu-id="86083-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86083-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86083-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86083-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sectionGroups/{id}/sections
POST /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
POST /groups/{id}/onenote/sectionGroups/{id}/sections
POST /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="request-headers"></a><span data-ttu-id="86083-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86083-115">Request headers</span></span>
| <span data-ttu-id="86083-116">Name</span><span class="sxs-lookup"><span data-stu-id="86083-116">Name</span></span>       | <span data-ttu-id="86083-117">Typ</span><span class="sxs-lookup"><span data-stu-id="86083-117">Type</span></span> | <span data-ttu-id="86083-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86083-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="86083-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="86083-119">Authorization</span></span>  | <span data-ttu-id="86083-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86083-120">string</span></span>  | <span data-ttu-id="86083-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="86083-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86083-123">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="86083-123">Content-Type</span></span> | <span data-ttu-id="86083-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86083-124">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="86083-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86083-125">Request body</span></span>
<span data-ttu-id="86083-126">Geben Sie im Anforderungstext einen Namen für den Abschnitt an.</span><span class="sxs-lookup"><span data-stu-id="86083-126">In the request body, supply a name for the section.</span></span>

<span data-ttu-id="86083-p103">Innerhalb der gleichen Hierarchieebene müssen Abschnittsnamen eindeutig sein. Der Name darf nicht mehr als 50 Zeichen und keines der folgenden Zeichen enthalten: ?\*\/:<>|&#''%~</span><span class="sxs-lookup"><span data-stu-id="86083-p103">Within the same hierarchy level, section names must be unique. The name cannot contain more than 50 characters or contain the following characters:  ?\*\/:<>|&#''%~</span></span>

## <a name="response"></a><span data-ttu-id="86083-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="86083-129">Response</span></span>

<span data-ttu-id="86083-130">Bei erfolgreicher Ausführung gibt die Methode den `201 Created` Antwortcode und ein [onenoteSection](../resources/section.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="86083-130">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/section.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86083-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86083-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86083-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86083-132">Request</span></span>
<span data-ttu-id="86083-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86083-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_section_from_sectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
Content-type: application/json
Content-length: 27

{
  "displayName": "Section name"
}
```

##### <a name="response"></a><span data-ttu-id="86083-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="86083-134">Response</span></span>
<span data-ttu-id="86083-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86083-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
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