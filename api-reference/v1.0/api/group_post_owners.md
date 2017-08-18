# <a name="add-group-owner"></a><span data-ttu-id="d1544-101">Gruppenbesitzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="d1544-101">Add group owner</span></span>
<span data-ttu-id="d1544-p101">Fügt einen Benutzer zu den Besitzern der Gruppe hinzu. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.</span><span class="sxs-lookup"><span data-stu-id="d1544-p101">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1544-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="d1544-104">Prerequisites</span></span>
<span data-ttu-id="d1544-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All* oder *Directory.ReadWrite.All* oder *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="d1544-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="d1544-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1544-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d1544-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d1544-107">Request headers</span></span>
| <span data-ttu-id="d1544-108">Name</span><span class="sxs-lookup"><span data-stu-id="d1544-108">Name</span></span>       | <span data-ttu-id="d1544-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d1544-109">Type</span></span> | <span data-ttu-id="d1544-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1544-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d1544-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1544-111">Authorization</span></span>  | <span data-ttu-id="d1544-112">string</span><span class="sxs-lookup"><span data-stu-id="d1544-112">string</span></span>  | <span data-ttu-id="d1544-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d1544-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1544-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d1544-115">Request body</span></span>
<span data-ttu-id="d1544-116">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d1544-116">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="d1544-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1544-117">Response</span></span>

<span data-ttu-id="d1544-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1544-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1544-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d1544-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1544-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1544-121">Request</span></span>
<span data-ttu-id="d1544-122">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d1544-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="d1544-123">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="d1544-123">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="d1544-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1544-124">Response</span></span>
<span data-ttu-id="d1544-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1544-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
