# <a name="remove-owner"></a><span data-ttu-id="b9a76-101">Besitzer entfernen</span><span class="sxs-lookup"><span data-stu-id="b9a76-101">Remove owner</span></span>

<span data-ttu-id="b9a76-102">Verwenden Sie diese API, um einen Besitzer aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die owners-Navigationseigenschaft zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="b9a76-102">Use this API to remove an owner from an Office 365 group, a security group or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9a76-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b9a76-103">Permissions</span></span>
<span data-ttu-id="b9a76-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9a76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="b9a76-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9a76-106">Permission type</span></span>      | <span data-ttu-id="b9a76-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9a76-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b9a76-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9a76-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b9a76-109">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9a76-109">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="b9a76-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9a76-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9a76-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9a76-111">Not supported.</span></span>    | 
|<span data-ttu-id="b9a76-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9a76-112">Application</span></span> | <span data-ttu-id="b9a76-113">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9a76-113">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b9a76-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9a76-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b9a76-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9a76-115">Request headers</span></span>
| <span data-ttu-id="b9a76-116">Name</span><span class="sxs-lookup"><span data-stu-id="b9a76-116">Name</span></span>       | <span data-ttu-id="b9a76-117">Typ</span><span class="sxs-lookup"><span data-stu-id="b9a76-117">Type</span></span> | <span data-ttu-id="b9a76-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9a76-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b9a76-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9a76-119">Authorization</span></span>  | <span data-ttu-id="b9a76-120">string</span><span class="sxs-lookup"><span data-stu-id="b9a76-120">string</span></span>  | <span data-ttu-id="b9a76-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b9a76-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9a76-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9a76-123">Request body</span></span>
<span data-ttu-id="b9a76-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b9a76-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9a76-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9a76-125">Response</span></span>

<span data-ttu-id="b9a76-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9a76-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9a76-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9a76-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9a76-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9a76-129">Request</span></span>
<span data-ttu-id="b9a76-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9a76-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="b9a76-131">Geben Sie in der Anforderung das `id` des Verzeichnisobjekts, das Sie entfernen möchten, nach dem $ref-Segment an.</span><span class="sxs-lookup"><span data-stu-id="b9a76-131">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

##### <a name="response"></a><span data-ttu-id="b9a76-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9a76-132">Response</span></span>
<span data-ttu-id="b9a76-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9a76-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
