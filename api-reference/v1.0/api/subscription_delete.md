# <a name="delete-subscription"></a><span data-ttu-id="82415-101">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="82415-101">Delete subscription</span></span>

<span data-ttu-id="82415-102">Löscht ein Abonnement.</span><span class="sxs-lookup"><span data-stu-id="82415-102">Delete a subscription.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82415-103">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="82415-103">Prerequisites</span></span>

<span data-ttu-id="82415-104">Die folgende Tabelle listet die vorgeschlagenen Berechtigungen, die für die jeweilige Ressource erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="82415-104">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="82415-105">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="82415-105">Resource type / Item</span></span>        | <span data-ttu-id="82415-106">Bereich</span><span class="sxs-lookup"><span data-stu-id="82415-106">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="82415-107">Kontakte</span><span class="sxs-lookup"><span data-stu-id="82415-107">Contacts</span></span>                    | <span data-ttu-id="82415-108">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="82415-108">Contacts.Read</span></span>       |
| <span data-ttu-id="82415-109">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="82415-109">Conversations</span></span>               | <span data-ttu-id="82415-110">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="82415-110">Group.Read.All</span></span>      |
| <span data-ttu-id="82415-111">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="82415-111">Events</span></span>                      | <span data-ttu-id="82415-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="82415-112">Calendars.Read</span></span>      |
| <span data-ttu-id="82415-113">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="82415-113">Messages</span></span>                    | <span data-ttu-id="82415-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="82415-114">Mail.Read</span></span>           |
| <span data-ttu-id="82415-115">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="82415-115">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="82415-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="82415-116">Files.ReadWrite</span></span>     |
| <span data-ttu-id="82415-117">Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="82415-117">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="82415-118">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82415-118">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82415-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="82415-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a><span data-ttu-id="82415-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="82415-120">Request headers</span></span>
| <span data-ttu-id="82415-121">Name</span><span class="sxs-lookup"><span data-stu-id="82415-121">Name</span></span>       | <span data-ttu-id="82415-122">Typ</span><span class="sxs-lookup"><span data-stu-id="82415-122">Type</span></span> | <span data-ttu-id="82415-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82415-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="82415-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="82415-124">Authorization</span></span>  | <span data-ttu-id="82415-125">string</span><span class="sxs-lookup"><span data-stu-id="82415-125">string</span></span>  | <span data-ttu-id="82415-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="82415-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82415-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="82415-128">Request body</span></span>
<span data-ttu-id="82415-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="82415-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82415-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="82415-130">Response</span></span>

<span data-ttu-id="82415-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82415-131">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="82415-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="82415-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82415-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="82415-133">Request</span></span>
<span data-ttu-id="82415-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="82415-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="82415-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="82415-135">Response</span></span>
<span data-ttu-id="82415-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="82415-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
