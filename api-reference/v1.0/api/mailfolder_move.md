# <a name="mailfolder-move"></a><span data-ttu-id="a295e-101">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="a295e-101">mailFolder: move</span></span>

<span data-ttu-id="a295e-102">Mit dieser API können Sie ein Objekt des Typs „mailfolder“ samt seinen Inhalten in ein anderes Objekt des Typs „mailfolder“ verschieben.</span><span class="sxs-lookup"><span data-stu-id="a295e-102">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="a295e-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a295e-103">Permissions</span></span>

<span data-ttu-id="a295e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a295e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a295e-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a295e-106">Permission type</span></span> | <span data-ttu-id="a295e-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a295e-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="a295e-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a295e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a295e-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a295e-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a295e-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a295e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a295e-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a295e-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a295e-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a295e-112">Application</span></span> | <span data-ttu-id="a295e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a295e-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a295e-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a295e-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="a295e-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a295e-115">Request headers</span></span>

| <span data-ttu-id="a295e-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a295e-116">Header</span></span> | <span data-ttu-id="a295e-117">Wert</span><span class="sxs-lookup"><span data-stu-id="a295e-117">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="a295e-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a295e-118">Authorization</span></span> | <span data-ttu-id="a295e-119">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="a295e-119"></span></span> <span data-ttu-id="a295e-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a295e-120">Required.</span></span> |
| <span data-ttu-id="a295e-121">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="a295e-121">Content-Type</span></span> | <span data-ttu-id="a295e-122">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="a295e-122"></span></span> <span data-ttu-id="a295e-123">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a295e-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a295e-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a295e-124">Request body</span></span>

<span data-ttu-id="a295e-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="a295e-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a295e-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="a295e-126">Parameter</span></span> | <span data-ttu-id="a295e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="a295e-127">Type</span></span> | <span data-ttu-id="a295e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a295e-128">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="a295e-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="a295e-129">destinationId</span></span>|<span data-ttu-id="a295e-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a295e-130">String</span></span>|<span data-ttu-id="a295e-131">Die Ordner-ID oder ein bekannter Ordnername.</span><span class="sxs-lookup"><span data-stu-id="a295e-131">The destination folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="a295e-132">Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a295e-132">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="a295e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="a295e-133">Response</span></span>

<span data-ttu-id="a295e-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine [mailFolder](../resources/mailfolder.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a295e-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a295e-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a295e-135">Example</span></span>

<span data-ttu-id="a295e-136">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="a295e-136">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a295e-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a295e-137">Request</span></span>

<span data-ttu-id="a295e-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a295e-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a295e-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="a295e-139">Response</span></span>

<span data-ttu-id="a295e-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a295e-140">Here is an example of the response.</span></span>

> <span data-ttu-id="a295e-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a295e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
