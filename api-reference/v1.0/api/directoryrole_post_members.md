# <a name="add-directory-role-member"></a><span data-ttu-id="0a28f-101">Verzeichnisrollenmitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="0a28f-101">Add directory role member</span></span>

<span data-ttu-id="0a28f-102">Mit dieser API können Sie ein neues Verzeichnisrollenmitglied erstellen.</span><span class="sxs-lookup"><span data-stu-id="0a28f-102">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a28f-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0a28f-103">Permissions</span></span>
<span data-ttu-id="0a28f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0a28f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0a28f-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a28f-106">Permission type</span></span>      | <span data-ttu-id="0a28f-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a28f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a28f-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a28f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0a28f-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0a28f-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0a28f-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a28f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a28f-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a28f-111">Not supported.</span></span>    |
|<span data-ttu-id="0a28f-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a28f-112">Application</span></span> | <span data-ttu-id="0a28f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a28f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a28f-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a28f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="0a28f-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a28f-115">Request headers</span></span>
| <span data-ttu-id="0a28f-116">Name</span><span class="sxs-lookup"><span data-stu-id="0a28f-116">Name</span></span>       | <span data-ttu-id="0a28f-117">Typ</span><span class="sxs-lookup"><span data-stu-id="0a28f-117">Type</span></span> | <span data-ttu-id="0a28f-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a28f-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0a28f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a28f-119">Authorization</span></span>  | <span data-ttu-id="0a28f-120">string</span><span class="sxs-lookup"><span data-stu-id="0a28f-120">string</span></span>  | <span data-ttu-id="0a28f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0a28f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a28f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a28f-123">Content-Type</span></span>  | <span data-ttu-id="0a28f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0a28f-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a28f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0a28f-125">Request body</span></span>
<span data-ttu-id="0a28f-126">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="0a28f-126">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="0a28f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a28f-127">Response</span></span>

<span data-ttu-id="0a28f-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a28f-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0a28f-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a28f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a28f-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a28f-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="0a28f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a28f-131">Response</span></span>
<span data-ttu-id="0a28f-132">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="0a28f-132">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

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