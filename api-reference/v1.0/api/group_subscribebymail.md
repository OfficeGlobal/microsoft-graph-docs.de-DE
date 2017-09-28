# <a name="group-subscribebymail"></a><span data-ttu-id="b82ef-101">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="b82ef-101">group: subscribeByMail</span></span>

<span data-ttu-id="b82ef-p101">Durch Aufrufen dieser Methode wird ermöglicht, dass der aktuelle Benutzer E-Mail-Benachrichtigungen für diese Gruppe über neue Beiträge, Ereignisse und Dateien in dieser Gruppe erhält. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b82ef-p101">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="b82ef-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b82ef-104">Permissions</span></span>
<span data-ttu-id="b82ef-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b82ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="b82ef-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b82ef-107">Permission type</span></span>      | <span data-ttu-id="b82ef-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b82ef-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b82ef-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b82ef-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b82ef-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b82ef-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b82ef-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b82ef-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b82ef-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b82ef-112">Not supported.</span></span>    |
|<span data-ttu-id="b82ef-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b82ef-113">Application</span></span> | <span data-ttu-id="b82ef-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b82ef-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b82ef-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b82ef-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="b82ef-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b82ef-116">Request headers</span></span>
| <span data-ttu-id="b82ef-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b82ef-117">Header</span></span>       | <span data-ttu-id="b82ef-118">Wert</span><span class="sxs-lookup"><span data-stu-id="b82ef-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b82ef-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b82ef-119">Authorization</span></span>  | <span data-ttu-id="b82ef-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b82ef-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b82ef-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b82ef-122">Request body</span></span>
<span data-ttu-id="b82ef-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b82ef-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b82ef-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="b82ef-124">Response</span></span>
<span data-ttu-id="b82ef-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b82ef-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b82ef-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b82ef-127">Example</span></span>
<span data-ttu-id="b82ef-128">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="b82ef-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b82ef-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b82ef-129">Request</span></span>
<span data-ttu-id="b82ef-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b82ef-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

##### <a name="response"></a><span data-ttu-id="b82ef-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b82ef-131">Response</span></span>
<span data-ttu-id="b82ef-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b82ef-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->