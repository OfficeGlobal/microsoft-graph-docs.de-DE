# <a name="delete-directoryobject"></a><span data-ttu-id="938b3-101">directoryObject löschen</span><span class="sxs-lookup"><span data-stu-id="938b3-101">Delete directoryObject</span></span>

<span data-ttu-id="938b3-102">Dient zum Löschen eines directoryObject.</span><span class="sxs-lookup"><span data-stu-id="938b3-102">Deletes a directoryObject.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="938b3-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="938b3-103">Prerequisites</span></span>
<span data-ttu-id="938b3-104">Der folgende **Bereich** ist erforderlich, um diese API auszuführen: _Directory.AccessAsUser.All_</span><span class="sxs-lookup"><span data-stu-id="938b3-104">The following **scopes** is required to execute this API: _Directory.AccessAsUser.All_</span></span>

<span data-ttu-id="938b3-p101">**HINWEIS:** Benutzer, Gruppen und Kontakte sind Typen von Verzeichnisobjekten. Wenn Sie Benutzer löschen müssen, kann und sollte daher der folgende **Bereich** verwendet werden: _User.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="938b3-p101">**NOTE:** Users, groups, and contacts are types of directory object. As a result,if you need to delete users, the following **scope** can and should be used: _User.ReadWrite.All_</span></span>
## <a name="http-request"></a><span data-ttu-id="938b3-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="938b3-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="938b3-108">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="938b3-108">Request headers</span></span>
| <span data-ttu-id="938b3-109">Name</span><span class="sxs-lookup"><span data-stu-id="938b3-109">Name</span></span>       | <span data-ttu-id="938b3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="938b3-110">Type</span></span> | <span data-ttu-id="938b3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="938b3-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="938b3-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="938b3-112">Authorization</span></span>  | <span data-ttu-id="938b3-113">string</span><span class="sxs-lookup"><span data-stu-id="938b3-113">string</span></span>  | <span data-ttu-id="938b3-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="938b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="938b3-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="938b3-116">Request body</span></span>
<span data-ttu-id="938b3-117">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="938b3-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="938b3-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="938b3-118">Response</span></span>

<span data-ttu-id="938b3-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="938b3-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="938b3-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="938b3-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="938b3-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="938b3-122">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObject/{id}
```
##### <a name="response"></a><span data-ttu-id="938b3-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="938b3-123">Response</span></span>

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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->