# <a name="group-resetunseencount"></a><span data-ttu-id="efb59-101">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="efb59-101">group: resetUnseenCount</span></span>

<span data-ttu-id="efb59-p101">Dient zum Zurücksetzen des unseenCount-Elements aller Beiträge, die der aktuelle Benutzer seit dem letzten Besuch noch nicht gesehen hat. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="efb59-p101">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for only Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efb59-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="efb59-104">Prerequisites</span></span>
<span data-ttu-id="efb59-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="efb59-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span> 
## <a name="http-request"></a><span data-ttu-id="efb59-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="efb59-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="efb59-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="efb59-107">Request headers</span></span>
| <span data-ttu-id="efb59-108">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="efb59-108">Header</span></span>       | <span data-ttu-id="efb59-109">Wert</span><span class="sxs-lookup"><span data-stu-id="efb59-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="efb59-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="efb59-110">Authorization</span></span>  | <span data-ttu-id="efb59-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="efb59-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="efb59-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="efb59-113">Request body</span></span>
<span data-ttu-id="efb59-114">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="efb59-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efb59-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="efb59-115">Response</span></span>

<span data-ttu-id="efb59-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="efb59-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efb59-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="efb59-118">Example</span></span>
<span data-ttu-id="efb59-119">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="efb59-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="efb59-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="efb59-120">Request</span></span>
<span data-ttu-id="efb59-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="efb59-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

##### <a name="response"></a><span data-ttu-id="efb59-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="efb59-122">Response</span></span>
<span data-ttu-id="efb59-123">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="efb59-123">Here is an example of the response.</span></span> 
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
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
