# <a name="group-removefavorite"></a><span data-ttu-id="29c04-101">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="29c04-101">group: removeFavorite</span></span>
<span data-ttu-id="29c04-p101">Entfernt die Gruppe aus der Liste der Favoritengruppen des aktuellen Benutzers. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="29c04-p101">Remove the group from the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="29c04-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="29c04-104">Permissions</span></span>
<span data-ttu-id="29c04-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="29c04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="29c04-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29c04-107">Permission type</span></span>      | <span data-ttu-id="29c04-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29c04-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="29c04-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29c04-109">Delegated (work or school account)</span></span> | <span data-ttu-id="29c04-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29c04-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="29c04-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29c04-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29c04-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29c04-112">Not supported.</span></span>    | 
|<span data-ttu-id="29c04-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29c04-113">Application</span></span> | <span data-ttu-id="29c04-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29c04-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="29c04-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29c04-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```
## <a name="request-headers"></a><span data-ttu-id="29c04-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29c04-116">Request headers</span></span>
| <span data-ttu-id="29c04-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="29c04-117">Header</span></span>       | <span data-ttu-id="29c04-118">Wert</span><span class="sxs-lookup"><span data-stu-id="29c04-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29c04-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="29c04-119">Authorization</span></span>  | <span data-ttu-id="29c04-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29c04-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29c04-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29c04-122">Request body</span></span>
<span data-ttu-id="29c04-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="29c04-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29c04-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="29c04-124">Response</span></span>

<span data-ttu-id="29c04-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29c04-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29c04-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29c04-127">Example</span></span>
<span data-ttu-id="29c04-128">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="29c04-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="29c04-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29c04-129">Request</span></span>
<span data-ttu-id="29c04-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29c04-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/removeFavorite
```

##### <a name="response"></a><span data-ttu-id="29c04-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="29c04-131">Response</span></span>
<span data-ttu-id="29c04-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29c04-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->