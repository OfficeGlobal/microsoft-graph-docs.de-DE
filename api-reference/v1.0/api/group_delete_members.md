# <a name="remove-member"></a><span data-ttu-id="527d8-101">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="527d8-101">Remove member</span></span>

<span data-ttu-id="527d8-p101">Verwenden Sie diese API, um ein Mitglied aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **members**-Navigationseigenschaft zu entfernen. Sie können Benutzer oder andere Gruppen entfernen.</span><span class="sxs-lookup"><span data-stu-id="527d8-p101">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="527d8-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="527d8-104">Prerequisites</span></span>
<span data-ttu-id="527d8-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All* oder *Directory.ReadWrite.All* oder *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="527d8-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="527d8-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="527d8-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="527d8-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="527d8-107">Request headers</span></span>
| <span data-ttu-id="527d8-108">Name</span><span class="sxs-lookup"><span data-stu-id="527d8-108">Name</span></span>       | <span data-ttu-id="527d8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="527d8-109">Type</span></span> | <span data-ttu-id="527d8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="527d8-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="527d8-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="527d8-111">Authorization</span></span>  | <span data-ttu-id="527d8-112">string</span><span class="sxs-lookup"><span data-stu-id="527d8-112">string</span></span>  | <span data-ttu-id="527d8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="527d8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="527d8-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="527d8-115">Request body</span></span>
<span data-ttu-id="527d8-116">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="527d8-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="527d8-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="527d8-117">Response</span></span>

<span data-ttu-id="527d8-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="527d8-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="527d8-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="527d8-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="527d8-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="527d8-121">Request</span></span>
<span data-ttu-id="527d8-122">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="527d8-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="527d8-123">Geben Sie in der Anforderung das `id` des Verzeichnisobjekts, das Sie entfernen möchten, nach dem $ref-Segment an.</span><span class="sxs-lookup"><span data-stu-id="527d8-123">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

##### <a name="response"></a><span data-ttu-id="527d8-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="527d8-124">Response</span></span>
<span data-ttu-id="527d8-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="527d8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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