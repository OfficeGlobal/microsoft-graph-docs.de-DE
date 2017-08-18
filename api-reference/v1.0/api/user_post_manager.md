# <a name="assign-a-manager"></a><span data-ttu-id="2cade-101">Einen Vorgesetzten zuweisen</span><span class="sxs-lookup"><span data-stu-id="2cade-101">Assign a manager</span></span>

<span data-ttu-id="2cade-102">Verwenden Sie diese API, um den Vorgesetzten eines Benutzers zuzuweisen.</span><span class="sxs-lookup"><span data-stu-id="2cade-102">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="2cade-103">Hinweis: Es ist nicht möglich, direkte Unterstellte zuzuweisen, verwenden Sie stattdessen diese API.</span><span class="sxs-lookup"><span data-stu-id="2cade-103">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cade-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="2cade-104">Prerequisites</span></span>
<span data-ttu-id="2cade-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Directory.ReadWrite.All* oder *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="2cade-105">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="2cade-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2cade-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2cade-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2cade-107">Request headers</span></span>
| <span data-ttu-id="2cade-108">Name</span><span class="sxs-lookup"><span data-stu-id="2cade-108">Name</span></span>       | <span data-ttu-id="2cade-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2cade-109">Type</span></span> | <span data-ttu-id="2cade-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2cade-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2cade-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cade-111">Authorization</span></span>  | <span data-ttu-id="2cade-112">string</span><span class="sxs-lookup"><span data-stu-id="2cade-112">string</span></span>  | <span data-ttu-id="2cade-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2cade-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cade-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2cade-115">Request body</span></span>
<span data-ttu-id="2cade-116">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="2cade-116">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="2cade-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="2cade-117">Response</span></span>

<span data-ttu-id="2cade-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2cade-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cade-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2cade-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2cade-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2cade-121">Request</span></span>
<span data-ttu-id="2cade-122">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2cade-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="2cade-123">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="2cade-123">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="2cade-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="2cade-124">Response</span></span>
<span data-ttu-id="2cade-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2cade-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
