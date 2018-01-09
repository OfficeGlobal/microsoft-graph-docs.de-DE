# <a name="remove-member"></a><span data-ttu-id="aeaf5-101">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="aeaf5-101">Remove member</span></span>
<span data-ttu-id="aeaf5-p101">Verwenden Sie diese API, um ein Mitglied aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **members**-Navigationseigenschaft zu entfernen. Sie können Benutzer oder andere Gruppen entfernen.</span><span class="sxs-lookup"><span data-stu-id="aeaf5-p101">Use this API to remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="aeaf5-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aeaf5-104">Permissions</span></span>
<span data-ttu-id="aeaf5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aeaf5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aeaf5-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aeaf5-107">Permission type</span></span>      | <span data-ttu-id="aeaf5-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aeaf5-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aeaf5-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aeaf5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="aeaf5-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aeaf5-110">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aeaf5-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aeaf5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aeaf5-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aeaf5-112">Not supported.</span></span>    |
|<span data-ttu-id="aeaf5-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aeaf5-113">Application</span></span> | <span data-ttu-id="aeaf5-114">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aeaf5-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="aeaf5-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aeaf5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="aeaf5-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aeaf5-116">Request headers</span></span>
| <span data-ttu-id="aeaf5-117">Name</span><span class="sxs-lookup"><span data-stu-id="aeaf5-117">Name</span></span>       | <span data-ttu-id="aeaf5-118">Typ</span><span class="sxs-lookup"><span data-stu-id="aeaf5-118">Type</span></span> | <span data-ttu-id="aeaf5-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aeaf5-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aeaf5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="aeaf5-120">Authorization</span></span>  | <span data-ttu-id="aeaf5-121">string</span><span class="sxs-lookup"><span data-stu-id="aeaf5-121">string</span></span>  | <span data-ttu-id="aeaf5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aeaf5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aeaf5-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aeaf5-124">Request body</span></span>
<span data-ttu-id="aeaf5-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aeaf5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aeaf5-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="aeaf5-126">Response</span></span>
<span data-ttu-id="aeaf5-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aeaf5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aeaf5-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aeaf5-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="aeaf5-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aeaf5-130">Request</span></span>
<span data-ttu-id="aeaf5-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aeaf5-131">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="aeaf5-132">Geben Sie in der Anforderung das `id` des Verzeichnisobjekts, das Sie entfernen möchten, nach dem $ref-Segment an.</span><span class="sxs-lookup"><span data-stu-id="aeaf5-132">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="aeaf5-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="aeaf5-133">Response</span></span>
<span data-ttu-id="aeaf5-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aeaf5-134">Here is an example of the response.</span></span>
><span data-ttu-id="aeaf5-135">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="aeaf5-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aeaf5-136">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="aeaf5-136">All the properties will be returned from an actual call.</span></span>
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