# <a name="mailfolder-move"></a><span data-ttu-id="4a517-101">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="4a517-101">mailFolder: move</span></span>

<span data-ttu-id="4a517-102">Mit dieser API können Sie ein Objekt des Typs „mailfolder“ samt seinen Inhalten in ein anderes Objekt des Typs „mailfolder“ verschieben.</span><span class="sxs-lookup"><span data-stu-id="4a517-102">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a517-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4a517-103">Permissions</span></span>
<span data-ttu-id="4a517-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a517-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a517-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a517-106">Permission type</span></span>      | <span data-ttu-id="4a517-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a517-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a517-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a517-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4a517-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a517-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4a517-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a517-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a517-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a517-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4a517-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a517-112">Application</span></span> | <span data-ttu-id="4a517-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a517-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a517-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a517-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="4a517-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a517-115">Request headers</span></span>
| <span data-ttu-id="4a517-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4a517-116">Header</span></span>       | <span data-ttu-id="4a517-117">Wert</span><span class="sxs-lookup"><span data-stu-id="4a517-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a517-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a517-118">Authorization</span></span>  | <span data-ttu-id="4a517-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4a517-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4a517-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a517-121">Content-Type</span></span>  | <span data-ttu-id="4a517-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="4a517-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a517-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a517-124">Request body</span></span>
<span data-ttu-id="4a517-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4a517-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4a517-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="4a517-126">Parameter</span></span>    | <span data-ttu-id="4a517-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4a517-127">Type</span></span>   |<span data-ttu-id="4a517-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a517-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a517-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="4a517-129">destinationId</span></span>|<span data-ttu-id="4a517-130">String</span><span class="sxs-lookup"><span data-stu-id="4a517-130">String</span></span>|<span data-ttu-id="4a517-131">Die Ordner-ID oder ein bekannter Ordnername wie *Posteingang*, *Entwürfe*, *Gesendete Objekte* oder *Gelöschte Objekte*.</span><span class="sxs-lookup"><span data-stu-id="4a517-131">The folder ID, or a well-known folder name such as *Inbox*, *Drafts*, *SentItems*, or *DeletedItems*.</span></span> <span data-ttu-id="4a517-132">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="4a517-132">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="4a517-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a517-133">Response</span></span>

<span data-ttu-id="4a517-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a517-134">If successful, this method returns `200 OK` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a517-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a517-135">Example</span></span>
<span data-ttu-id="4a517-136">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4a517-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4a517-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a517-137">Request</span></span>
<span data-ttu-id="4a517-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a517-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="4a517-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a517-139">Response</span></span>
<span data-ttu-id="4a517-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a517-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
