# <a name="create-mailfolder"></a><span data-ttu-id="889d5-101">MailFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="889d5-101">Create MailFolder</span></span>

<span data-ttu-id="889d5-102">Mit dieser API können Sie neue untergeordnete Objekte des Typs „mailfolder“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="889d5-102">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="889d5-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="889d5-103">Permissions</span></span>

<span data-ttu-id="889d5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="889d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="889d5-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="889d5-106">Permission type</span></span> | <span data-ttu-id="889d5-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="889d5-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="889d5-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="889d5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="889d5-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="889d5-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="889d5-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="889d5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="889d5-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="889d5-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="889d5-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="889d5-112">Application</span></span> | <span data-ttu-id="889d5-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="889d5-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="889d5-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="889d5-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="889d5-115">Geben Sie den übergeordneten Ordner oder einen bekannten Ordnernamen in der Abfrage-URL als Ordner-ID an.</span><span class="sxs-lookup"><span data-stu-id="889d5-115">Specify the parent folder in the query URL as a folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="889d5-116">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="889d5-116">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="889d5-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="889d5-117">Request headers</span></span>

| <span data-ttu-id="889d5-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="889d5-118">Header</span></span> | <span data-ttu-id="889d5-119">Wert</span><span class="sxs-lookup"><span data-stu-id="889d5-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="889d5-120">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="889d5-120">Authorization</span></span> | <span data-ttu-id="889d5-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="889d5-121"></span></span> <span data-ttu-id="889d5-122">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="889d5-122">Required.</span></span> |
| <span data-ttu-id="889d5-123">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="889d5-123">Content-Type</span></span> | <span data-ttu-id="889d5-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="889d5-124"></span></span> <span data-ttu-id="889d5-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="889d5-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="889d5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="889d5-126">Request body</span></span>

<span data-ttu-id="889d5-127">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="889d5-127">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="889d5-128">**DisplayName** ist die einzige schreibbare Eigenschaft eines [mailFolder](../resources/mailfolder.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="889d5-128">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="889d5-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="889d5-129">Parameter</span></span> | <span data-ttu-id="889d5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="889d5-130">Type</span></span> | <span data-ttu-id="889d5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="889d5-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="889d5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="889d5-132">displayName</span></span>|<span data-ttu-id="889d5-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="889d5-133">String</span></span>|<span data-ttu-id="889d5-134">Der Anzeigename für den neuen Ordner.</span><span class="sxs-lookup"><span data-stu-id="889d5-134">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="889d5-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="889d5-135">Response</span></span>

<span data-ttu-id="889d5-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und eine [mailFolder](../resources/mailfolder.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="889d5-136">If successful, this method returns a `201 Created` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="889d5-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="889d5-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="889d5-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="889d5-138">Request</span></span>

<span data-ttu-id="889d5-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="889d5-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="889d5-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="889d5-140">Response</span></span>
<span data-ttu-id="889d5-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="889d5-141">Here is an example of the response.</span></span>

> <span data-ttu-id="889d5-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="889d5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
