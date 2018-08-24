# <a name="message-copy"></a><span data-ttu-id="a9ce2-101">message: Text</span><span class="sxs-lookup"><span data-stu-id="a9ce2-101">message: copy</span></span>

<span data-ttu-id="a9ce2-102">Mit dieser API können Sie Nachrichten in Ordner kopieren.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-102">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9ce2-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a9ce2-103">Permissions</span></span>

<span data-ttu-id="a9ce2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9ce2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a9ce2-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a9ce2-106">Permission type</span></span> | <span data-ttu-id="a9ce2-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a9ce2-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="a9ce2-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a9ce2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a9ce2-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9ce2-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a9ce2-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a9ce2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9ce2-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9ce2-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a9ce2-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a9ce2-112">Application</span></span> | <span data-ttu-id="a9ce2-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9ce2-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9ce2-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9ce2-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="a9ce2-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a9ce2-115">Request headers</span></span>

| <span data-ttu-id="a9ce2-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a9ce2-116">Header</span></span> | <span data-ttu-id="a9ce2-117">Wert</span><span class="sxs-lookup"><span data-stu-id="a9ce2-117">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="a9ce2-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a9ce2-118">Authorization</span></span> | <span data-ttu-id="a9ce2-119">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-119"></span></span> <span data-ttu-id="a9ce2-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-120">Required.</span></span> |
| <span data-ttu-id="a9ce2-121">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="a9ce2-121">Content-Type</span></span> | <span data-ttu-id="a9ce2-122">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-122"></span></span> <span data-ttu-id="a9ce2-123">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9ce2-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a9ce2-124">Request body</span></span>

<span data-ttu-id="a9ce2-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a9ce2-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="a9ce2-126">Parameter</span></span> | <span data-ttu-id="a9ce2-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a9ce2-127">Type</span></span> | <span data-ttu-id="a9ce2-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9ce2-128">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="a9ce2-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="a9ce2-129">destinationId</span></span>|<span data-ttu-id="a9ce2-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a9ce2-130">String</span></span>|<span data-ttu-id="a9ce2-131">Die Zielordner-ID oder ein bekannter Ordnername.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-131">The destination folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="a9ce2-132">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [MailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a9ce2-132">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="a9ce2-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9ce2-133">Response</span></span>

<span data-ttu-id="a9ce2-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und eine [mailFolder](../resources/message.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-134">If successful, this method returns a `201 Created` response code and a [sharedDriveItem](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9ce2-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a9ce2-135">Example</span></span>

<span data-ttu-id="a9ce2-136">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-136">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a9ce2-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a9ce2-137">Request</span></span>
<span data-ttu-id="a9ce2-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="a9ce2-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a9ce2-139">Response</span></span>

<span data-ttu-id="a9ce2-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-140">Here is an example of the response.</span></span>

> <span data-ttu-id="a9ce2-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a9ce2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
