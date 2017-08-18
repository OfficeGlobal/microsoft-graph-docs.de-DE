# <a name="group-subscribebymail"></a><span data-ttu-id="baf66-101">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="baf66-101">group: subscribeByMail</span></span>

<span data-ttu-id="baf66-p101">Durch Aufrufen dieser Methode wird ermöglicht, dass der aktuelle Benutzer E-Mail-Benachrichtigungen für diese Gruppe über neue Beiträge, Ereignisse und Dateien in dieser Gruppe erhält. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="baf66-p101">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for only Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="baf66-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="baf66-104">Prerequisites</span></span>
<span data-ttu-id="baf66-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All* 
*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="baf66-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All* 
*Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="baf66-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="baf66-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="baf66-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="baf66-107">Request headers</span></span>
| <span data-ttu-id="baf66-108">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="baf66-108">Header</span></span>       | <span data-ttu-id="baf66-109">Wert</span><span class="sxs-lookup"><span data-stu-id="baf66-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="baf66-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="baf66-110">Authorization</span></span>  | <span data-ttu-id="baf66-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="baf66-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="baf66-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="baf66-113">Request body</span></span>

## <a name="response"></a><span data-ttu-id="baf66-114">Antwort</span><span class="sxs-lookup"><span data-stu-id="baf66-114">Response</span></span>

<span data-ttu-id="baf66-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="baf66-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baf66-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="baf66-117">Example</span></span>
<span data-ttu-id="baf66-118">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="baf66-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="baf66-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="baf66-119">Request</span></span>
<span data-ttu-id="baf66-120">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="baf66-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

##### <a name="response"></a><span data-ttu-id="baf66-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="baf66-121">Response</span></span>
<span data-ttu-id="baf66-122">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="baf66-122">Here is an example of the response.</span></span> 
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