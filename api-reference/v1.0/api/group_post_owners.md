# <a name="add-group-owner"></a><span data-ttu-id="18c62-101">Gruppenbesitzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="18c62-101">Add group owner</span></span>
<span data-ttu-id="18c62-p101">Fügt einen Benutzer zu den Besitzern der Gruppe hinzu. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind, die das Gruppenobjekt ändern können.</span><span class="sxs-lookup"><span data-stu-id="18c62-p101">Add a user to the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="18c62-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18c62-104">Permissions</span></span>
<span data-ttu-id="18c62-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="18c62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="18c62-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18c62-107">Permission type</span></span>      | <span data-ttu-id="18c62-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18c62-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18c62-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18c62-109">Delegated (work or school account)</span></span> | <span data-ttu-id="18c62-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18c62-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="18c62-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18c62-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18c62-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="18c62-112">Not supported.</span></span>    |
|<span data-ttu-id="18c62-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18c62-113">Application</span></span> | <span data-ttu-id="18c62-114">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18c62-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18c62-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18c62-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/owners/$ref
```
## <a name="request-headers"></a><span data-ttu-id="18c62-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18c62-116">Request headers</span></span>
| <span data-ttu-id="18c62-117">Name</span><span class="sxs-lookup"><span data-stu-id="18c62-117">Name</span></span>       | <span data-ttu-id="18c62-118">Typ</span><span class="sxs-lookup"><span data-stu-id="18c62-118">Type</span></span> | <span data-ttu-id="18c62-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18c62-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18c62-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="18c62-120">Authorization</span></span>  | <span data-ttu-id="18c62-121">string</span><span class="sxs-lookup"><span data-stu-id="18c62-121">string</span></span>  | <span data-ttu-id="18c62-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18c62-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18c62-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18c62-124">Request body</span></span>
<span data-ttu-id="18c62-125">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="18c62-125">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="18c62-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="18c62-126">Response</span></span>

<span data-ttu-id="18c62-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18c62-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18c62-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18c62-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18c62-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18c62-130">Request</span></span>
<span data-ttu-id="18c62-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18c62-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="18c62-132">Geben Sie im Anforderungstext eine JSON-Darstellung eines [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="18c62-132">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="18c62-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="18c62-133">Response</span></span>
<span data-ttu-id="18c62-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18c62-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
