# <a name="create-mailfolder"></a><span data-ttu-id="9f8d1-101">MailFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="9f8d1-101">Create MailFolder</span></span>

<span data-ttu-id="9f8d1-102">Mit dieser API können Sie neue untergeordnete Objekte des Typs „mailfolder“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="9f8d1-102">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f8d1-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f8d1-103">Permissions</span></span>
<span data-ttu-id="9f8d1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f8d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9f8d1-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f8d1-106">Permission type</span></span>      | <span data-ttu-id="9f8d1-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f8d1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f8d1-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f8d1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9f8d1-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f8d1-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f8d1-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f8d1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f8d1-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f8d1-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9f8d1-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f8d1-112">Application</span></span> | <span data-ttu-id="9f8d1-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f8d1-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f8d1-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f8d1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="9f8d1-115">Geben Sie den übergeordneten Ordner in der Abfrage-URL als eine Ordner-ID oder einen bekannten Ordnernamen wie *Posteingang*, *Entwürfe*, *Gesendete Objekte* oder *Gelöschte Objekte* an.</span><span class="sxs-lookup"><span data-stu-id="9f8d1-115">Specify the parent folder in the query URL as a folder ID, or a well-known folder name such as *Inbox*, *Drafts*, *SentItems*, or *DeletedItems*.</span></span> <span data-ttu-id="9f8d1-116">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9f8d1-116">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f8d1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f8d1-117">Request headers</span></span>
| <span data-ttu-id="9f8d1-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9f8d1-118">Header</span></span>       | <span data-ttu-id="9f8d1-119">Wert</span><span class="sxs-lookup"><span data-stu-id="9f8d1-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f8d1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f8d1-120">Authorization</span></span>  | <span data-ttu-id="9f8d1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f8d1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9f8d1-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f8d1-123">Content-Type</span></span>  | <span data-ttu-id="9f8d1-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="9f8d1-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f8d1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f8d1-126">Request body</span></span>
<span data-ttu-id="9f8d1-p105">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an. **displayName** ist die einzige schreibbare Eigenschaft für ein [MailFolder](../resources/mailfolder.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="9f8d1-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="9f8d1-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="9f8d1-129">Parameter</span></span>    | <span data-ttu-id="9f8d1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="9f8d1-130">Type</span></span>   |<span data-ttu-id="9f8d1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f8d1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f8d1-132">displayName</span><span class="sxs-lookup"><span data-stu-id="9f8d1-132">displayName</span></span>|<span data-ttu-id="9f8d1-133">String</span><span class="sxs-lookup"><span data-stu-id="9f8d1-133">String</span></span>|<span data-ttu-id="9f8d1-134">Der Anzeigename für den neuen Ordner.</span><span class="sxs-lookup"><span data-stu-id="9f8d1-134">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="9f8d1-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f8d1-135">Response</span></span>

<span data-ttu-id="9f8d1-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [MailFolder](../resources/mailfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f8d1-136">If successful, this method returns `201 Created` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f8d1-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f8d1-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f8d1-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f8d1-138">Request</span></span>
<span data-ttu-id="9f8d1-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f8d1-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9f8d1-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f8d1-140">Response</span></span>
<span data-ttu-id="9f8d1-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f8d1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
