# <a name="create-mailfolder"></a><span data-ttu-id="d7da2-101">MailFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="d7da2-101">Create MailFolder</span></span>

<span data-ttu-id="d7da2-102">Mit dieser API können Sie neue untergeordnete Objekte des Typs „mailfolder“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="d7da2-102">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7da2-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d7da2-103">Permissions</span></span>
<span data-ttu-id="d7da2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7da2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d7da2-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d7da2-106">Permission type</span></span>      | <span data-ttu-id="d7da2-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d7da2-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="d7da2-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d7da2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d7da2-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7da2-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="d7da2-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d7da2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7da2-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7da2-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="d7da2-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d7da2-112">Application</span></span> | <span data-ttu-id="d7da2-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7da2-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d7da2-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7da2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="d7da2-115">Geben Sie den übergeordneten Ordner in der Abfrage-URL als Ordner-ID an oder den bekannten Ordnernamen `Inbox`, `Drafts`, `SentItems` oder `DeletedItems`.</span><span class="sxs-lookup"><span data-stu-id="d7da2-115">Specify the parent folder in the query URL as a folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7da2-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d7da2-116">Request headers</span></span>
| <span data-ttu-id="d7da2-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d7da2-117">Header</span></span>       | <span data-ttu-id="d7da2-118">Wert</span><span class="sxs-lookup"><span data-stu-id="d7da2-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d7da2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7da2-119">Authorization</span></span>  | <span data-ttu-id="d7da2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d7da2-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d7da2-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7da2-122">Content-Type</span></span>  | <span data-ttu-id="d7da2-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="d7da2-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d7da2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d7da2-125">Request body</span></span>
<span data-ttu-id="d7da2-p104">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an. **displayName** ist die einzige schreibbare Eigenschaft für ein [MailFolder](../resources/mailfolder.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="d7da2-p104">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="d7da2-128">Parameter</span><span class="sxs-lookup"><span data-stu-id="d7da2-128">Parameter</span></span>    | <span data-ttu-id="d7da2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="d7da2-129">Type</span></span>   |<span data-ttu-id="d7da2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7da2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7da2-131">displayName</span><span class="sxs-lookup"><span data-stu-id="d7da2-131">displayName</span></span>|<span data-ttu-id="d7da2-132">String</span><span class="sxs-lookup"><span data-stu-id="d7da2-132">String</span></span>|<span data-ttu-id="d7da2-133">Der Anzeigename für den neuen Ordner.</span><span class="sxs-lookup"><span data-stu-id="d7da2-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="d7da2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7da2-134">Response</span></span>

<span data-ttu-id="d7da2-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7da2-135">If successful, this method returns `201, Created` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7da2-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d7da2-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7da2-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d7da2-137">Request</span></span>
<span data-ttu-id="d7da2-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d7da2-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

##### <a name="response"></a><span data-ttu-id="d7da2-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="d7da2-139">Response</span></span>
<span data-ttu-id="d7da2-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d7da2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
