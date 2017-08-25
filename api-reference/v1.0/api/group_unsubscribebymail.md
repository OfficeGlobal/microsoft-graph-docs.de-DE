# <a name="group-unsubscribebymail"></a><span data-ttu-id="2bb44-101">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="2bb44-101">group: unsubscribeByMail</span></span>

<span data-ttu-id="2bb44-p101">Durch Aufrufen dieser Methode wird verhindert, dass der aktuelle Benutzer E-Mail-Benachrichtigungen für diese Gruppe über neue Beiträge, Ereignisse und die Dateien in dieser Gruppe erhält. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2bb44-p101">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span> 
## <a name="permissions"></a><span data-ttu-id="2bb44-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2bb44-104">Permissions</span></span>
<span data-ttu-id="2bb44-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2bb44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="2bb44-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2bb44-107">Permission type</span></span>      | <span data-ttu-id="2bb44-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2bb44-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="2bb44-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2bb44-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2bb44-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bb44-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="2bb44-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2bb44-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bb44-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2bb44-112">Not supported.</span></span>    | 
|<span data-ttu-id="2bb44-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2bb44-113">Application</span></span> | <span data-ttu-id="2bb44-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bb44-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2bb44-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2bb44-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="2bb44-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2bb44-116">Request headers</span></span>
| <span data-ttu-id="2bb44-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2bb44-117">Header</span></span>       | <span data-ttu-id="2bb44-118">Wert</span><span class="sxs-lookup"><span data-stu-id="2bb44-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2bb44-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bb44-119">Authorization</span></span>  | <span data-ttu-id="2bb44-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2bb44-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2bb44-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2bb44-122">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2bb44-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="2bb44-123">Response</span></span>
<span data-ttu-id="2bb44-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2bb44-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bb44-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2bb44-126">Example</span></span>
<span data-ttu-id="2bb44-127">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="2bb44-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2bb44-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2bb44-128">Request</span></span>
<span data-ttu-id="2bb44-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2bb44-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```

##### <a name="response"></a><span data-ttu-id="2bb44-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="2bb44-130">Response</span></span>
<span data-ttu-id="2bb44-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2bb44-131">Here is an example of the response.</span></span> 
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
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
