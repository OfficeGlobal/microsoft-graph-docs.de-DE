# <a name="create-mailfolder"></a><span data-ttu-id="2a5b3-101">MailFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="2a5b3-101">Create MailFolder</span></span>

<span data-ttu-id="2a5b3-102">Verwenden Sie diese API, um einen neuen E-Mail-Ordner im Stammordner des Benutzerpostfachs zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="2a5b3-102">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a5b3-103">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="2a5b3-103">Prerequisites</span></span>
<span data-ttu-id="2a5b3-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="2a5b3-104">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="2a5b3-105">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a5b3-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="2a5b3-106">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a5b3-106">Request headers</span></span>
| <span data-ttu-id="2a5b3-107">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2a5b3-107">Header</span></span>       | <span data-ttu-id="2a5b3-108">Wert</span><span class="sxs-lookup"><span data-stu-id="2a5b3-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2a5b3-109">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a5b3-109">Authorization</span></span>  | <span data-ttu-id="2a5b3-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2a5b3-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2a5b3-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a5b3-112">Content-Type</span></span>  | <span data-ttu-id="2a5b3-113">application/json</span><span class="sxs-lookup"><span data-stu-id="2a5b3-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a5b3-114">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a5b3-114">Request body</span></span>
<span data-ttu-id="2a5b3-p102">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an. **displayName** ist die einzige schreibbare Eigenschaft für ein [MailFolder](../resources/mailfolder.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="2a5b3-p102">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="2a5b3-117">Parameter</span><span class="sxs-lookup"><span data-stu-id="2a5b3-117">Parameter</span></span>    | <span data-ttu-id="2a5b3-118">Typ</span><span class="sxs-lookup"><span data-stu-id="2a5b3-118">Type</span></span>   |<span data-ttu-id="2a5b3-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a5b3-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a5b3-120">displayName</span><span class="sxs-lookup"><span data-stu-id="2a5b3-120">displayName</span></span>|<span data-ttu-id="2a5b3-121">String</span><span class="sxs-lookup"><span data-stu-id="2a5b3-121">String</span></span>|<span data-ttu-id="2a5b3-122">Der Anzeigename für den neuen Ordner.</span><span class="sxs-lookup"><span data-stu-id="2a5b3-122">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="2a5b3-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a5b3-123">Response</span></span>

<span data-ttu-id="2a5b3-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a5b3-124">If successful, this method returns `201, Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a5b3-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a5b3-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a5b3-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a5b3-126">Request</span></span>
<span data-ttu-id="2a5b3-127">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a5b3-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="2a5b3-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a5b3-128">Response</span></span>
<span data-ttu-id="2a5b3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a5b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
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
