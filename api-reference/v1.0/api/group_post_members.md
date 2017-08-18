# <a name="add-member"></a><span data-ttu-id="9dd68-101">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="9dd68-101">Add member</span></span>

<span data-ttu-id="9dd68-p101">Verwenden Sie diese API, um ein Mitglied einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **member**-Navigationseigenschaft hinzuzufügen. Sie können Benutzer oder andere Gruppen hinzufügen. Wichtig: Sie können nur von Benutzern zu Office 365-Gruppen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="9dd68-p101">Use this API to add a member to an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can add users or other groups. Important: You can add only users to Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9dd68-105">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="9dd68-105">Prerequisites</span></span>
<span data-ttu-id="9dd68-106">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All* oder *Directory.ReadWrite.All* oder *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="9dd68-106">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="9dd68-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9dd68-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9dd68-108">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9dd68-108">Request headers</span></span>
| <span data-ttu-id="9dd68-109">Name</span><span class="sxs-lookup"><span data-stu-id="9dd68-109">Name</span></span>       | <span data-ttu-id="9dd68-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9dd68-110">Type</span></span> | <span data-ttu-id="9dd68-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dd68-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9dd68-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dd68-112">Authorization</span></span>  | <span data-ttu-id="9dd68-113">string</span><span class="sxs-lookup"><span data-stu-id="9dd68-113">string</span></span>  | <span data-ttu-id="9dd68-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9dd68-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9dd68-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9dd68-116">Request body</span></span>
<span data-ttu-id="9dd68-117">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)- oder [group](../resources/group.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9dd68-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="9dd68-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="9dd68-118">Response</span></span>

<span data-ttu-id="9dd68-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9dd68-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dd68-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9dd68-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9dd68-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9dd68-122">Request</span></span>
<span data-ttu-id="9dd68-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9dd68-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
<span data-ttu-id="9dd68-124">Geben Sie im Anforderungstext eine JSON-Darstellung des `id` des [directoryObject](../resources/directoryobject.md)-, [user](../resources/user.md)- oder [group](../resources/group.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="9dd68-124">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>
##### <a name="response"></a><span data-ttu-id="9dd68-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="9dd68-125">Response</span></span>
<span data-ttu-id="9dd68-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9dd68-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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