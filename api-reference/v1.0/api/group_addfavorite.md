# <a name="group-addfavorite"></a><span data-ttu-id="e1636-101">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="e1636-101">group: addFavorite</span></span>
<span data-ttu-id="e1636-p101">Fügt die Gruppe zu der Liste der Favoritengruppen des aktuellen Benutzers hinzu. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1636-p101">Add the group to the list of the current user's favorite groups. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1636-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e1636-104">Permissions</span></span>
<span data-ttu-id="e1636-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1636-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e1636-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1636-107">Permission type</span></span>      | <span data-ttu-id="e1636-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1636-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1636-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1636-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e1636-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1636-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1636-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1636-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1636-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1636-112">Not supported.</span></span>    |
|<span data-ttu-id="e1636-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1636-113">Application</span></span> | <span data-ttu-id="e1636-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1636-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1636-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1636-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="e1636-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1636-116">Request headers</span></span>
| <span data-ttu-id="e1636-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e1636-117">Header</span></span>       | <span data-ttu-id="e1636-118">Wert</span><span class="sxs-lookup"><span data-stu-id="e1636-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e1636-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e1636-119">Authorization</span></span>  | <span data-ttu-id="e1636-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1636-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1636-122">Prefer</span><span class="sxs-lookup"><span data-stu-id="e1636-122">Prefer</span></span> | <span data-ttu-id="e1636-123">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="e1636-123">return=minimal.</span></span> <span data-ttu-id="e1636-124">Wenn die Antwortkopfzeile „minimal“ in der Anforderungskopfzeile enthalten ist, gibt eine erfolgreiche Antwort den `204 No Content`-Code zurück. </span><span class="sxs-lookup"><span data-stu-id="e1636-124">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="e1636-125">Optional.</span><span class="sxs-lookup"><span data-stu-id="e1636-125">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1636-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1636-126">Request body</span></span>
<span data-ttu-id="e1636-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e1636-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1636-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1636-128">Response</span></span>
<span data-ttu-id="e1636-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1636-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1636-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1636-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e1636-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1636-132">Request</span></span>
<span data-ttu-id="e1636-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1636-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="e1636-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1636-134">Response</span></span>
<span data-ttu-id="e1636-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e1636-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
