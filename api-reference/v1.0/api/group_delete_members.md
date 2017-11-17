# <a name="remove-member"></a><span data-ttu-id="38704-101">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="38704-101">Remove member</span></span>

<span data-ttu-id="38704-p101">Verwenden Sie diese API, um ein Mitglied aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **members**-Navigationseigenschaft zu entfernen. Sie können Benutzer oder andere Gruppen entfernen.</span><span class="sxs-lookup"><span data-stu-id="38704-p101">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="38704-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="38704-104">Permissions</span></span>
<span data-ttu-id="38704-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="38704-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="38704-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38704-107">Permission type</span></span>      | <span data-ttu-id="38704-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38704-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38704-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38704-109">Delegated (work or school account)</span></span> | <span data-ttu-id="38704-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="38704-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="38704-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38704-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38704-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="38704-112">Not supported.</span></span>    |
|<span data-ttu-id="38704-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38704-113">Application</span></span> | <span data-ttu-id="38704-114">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38704-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38704-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38704-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="38704-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38704-116">Request headers</span></span>
| <span data-ttu-id="38704-117">Name</span><span class="sxs-lookup"><span data-stu-id="38704-117">Name</span></span>       | <span data-ttu-id="38704-118">Typ</span><span class="sxs-lookup"><span data-stu-id="38704-118">Type</span></span> | <span data-ttu-id="38704-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38704-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38704-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="38704-120">Authorization</span></span>  | <span data-ttu-id="38704-121">string</span><span class="sxs-lookup"><span data-stu-id="38704-121">string</span></span>  | <span data-ttu-id="38704-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="38704-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38704-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38704-124">Request body</span></span>
<span data-ttu-id="38704-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="38704-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38704-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="38704-126">Response</span></span>

<span data-ttu-id="38704-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38704-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38704-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38704-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38704-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38704-130">Request</span></span>
<span data-ttu-id="38704-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="38704-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="38704-132">Geben Sie in der Anforderung das `id` des Verzeichnisobjekts, das Sie entfernen möchten, nach dem $ref-Segment an.</span><span class="sxs-lookup"><span data-stu-id="38704-132">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

##### <a name="response"></a><span data-ttu-id="38704-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="38704-133">Response</span></span>
<span data-ttu-id="38704-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="38704-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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