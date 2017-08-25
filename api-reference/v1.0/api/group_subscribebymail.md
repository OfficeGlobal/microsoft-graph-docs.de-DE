# <a name="group-subscribebymail"></a><span data-ttu-id="3ac01-101">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="3ac01-101">group: subscribeByMail</span></span>

<span data-ttu-id="3ac01-p101">Durch Aufrufen dieser Methode wird ermöglicht, dass der aktuelle Benutzer E-Mail-Benachrichtigungen für diese Gruppe über neue Beiträge, Ereignisse und Dateien in dieser Gruppe erhält. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ac01-p101">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ac01-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3ac01-104">Permissions</span></span>
<span data-ttu-id="3ac01-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ac01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="3ac01-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ac01-107">Permission type</span></span>      | <span data-ttu-id="3ac01-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ac01-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="3ac01-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ac01-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3ac01-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ac01-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="3ac01-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ac01-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ac01-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ac01-112">Not supported.</span></span>    | 
|<span data-ttu-id="3ac01-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ac01-113">Application</span></span> | <span data-ttu-id="3ac01-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ac01-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3ac01-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ac01-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="3ac01-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ac01-116">Request headers</span></span>
| <span data-ttu-id="3ac01-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3ac01-117">Header</span></span>       | <span data-ttu-id="3ac01-118">Wert</span><span class="sxs-lookup"><span data-stu-id="3ac01-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3ac01-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ac01-119">Authorization</span></span>  | <span data-ttu-id="3ac01-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3ac01-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ac01-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ac01-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3ac01-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ac01-123">Response</span></span>
<span data-ttu-id="3ac01-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ac01-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ac01-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ac01-126">Example</span></span>
<span data-ttu-id="3ac01-127">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="3ac01-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3ac01-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ac01-128">Request</span></span>
<span data-ttu-id="3ac01-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ac01-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

##### <a name="response"></a><span data-ttu-id="3ac01-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ac01-130">Response</span></span>
<span data-ttu-id="3ac01-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3ac01-131">Here is an example of the response.</span></span> 
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