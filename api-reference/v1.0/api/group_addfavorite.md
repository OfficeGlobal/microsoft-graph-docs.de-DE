# <a name="group-addfavorite"></a><span data-ttu-id="85091-101">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="85091-101">group: addFavorite</span></span>
<span data-ttu-id="85091-p101">Fügt die Gruppe zu der Liste der Favoritengruppen des aktuellen Benutzers hinzu. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85091-p101">Add the group to the list of the current user's favorite groups. Supported for only Office 365 groups.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85091-104">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="85091-104">Prerequisites</span></span>
<span data-ttu-id="85091-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="85091-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="85091-106">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85091-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```
## <a name="request-headers"></a><span data-ttu-id="85091-107">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85091-107">Request headers</span></span>
| <span data-ttu-id="85091-108">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="85091-108">Header</span></span>       | <span data-ttu-id="85091-109">Wert</span><span class="sxs-lookup"><span data-stu-id="85091-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85091-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="85091-110">Authorization</span></span>  | <span data-ttu-id="85091-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="85091-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85091-113">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85091-113">Request body</span></span>
<span data-ttu-id="85091-114">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="85091-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85091-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="85091-115">Response</span></span>

<span data-ttu-id="85091-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85091-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85091-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85091-118">Example</span></span>
<span data-ttu-id="85091-119">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="85091-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="85091-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85091-120">Request</span></span>
<span data-ttu-id="85091-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85091-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

##### <a name="response"></a><span data-ttu-id="85091-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="85091-122">Response</span></span>
<span data-ttu-id="85091-123">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="85091-123">Here is an example of the response.</span></span>
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
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->