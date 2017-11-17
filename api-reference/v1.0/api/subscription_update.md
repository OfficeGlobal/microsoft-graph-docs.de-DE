# <a name="update-subscription"></a><span data-ttu-id="bdcee-101">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bdcee-101">Update subscription</span></span>

<span data-ttu-id="bdcee-102">Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="bdcee-102">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="bdcee-p101">Abonnements für Ressourcen laufen an Tagen ab, die von den einzelnen Ressourcentypen vorgegeben werden.  Um keine Benachrichtigungen zu verpassen, sollten Abonnements weit vor ihrem Ablaufdatum verlängert werden.  Informationen zu den einzelnen Ablaufdaten finden Sie unter [Abonnement](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="bdcee-p101">Subscriptions to resources expire at dates proscribed by the individual resource types.  In order not to miss notifications, subscriptions should be renewed well in advance of their expiry date.  See [subscription](../resources/subscription.md) for individual expiry dates.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdcee-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bdcee-106">Permissions</span></span>

<span data-ttu-id="bdcee-p102">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bdcee-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="bdcee-109">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="bdcee-109">Resource type / Item</span></span>        | <span data-ttu-id="bdcee-110">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="bdcee-110">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="bdcee-111">Kontakte</span><span class="sxs-lookup"><span data-stu-id="bdcee-111">Contacts</span></span>                    | <span data-ttu-id="bdcee-112">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bdcee-112">Contacts.Read</span></span>       |
| <span data-ttu-id="bdcee-113">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="bdcee-113">Conversations</span></span>               | <span data-ttu-id="bdcee-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdcee-114">Group.Read.All</span></span>      |
| <span data-ttu-id="bdcee-115">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="bdcee-115">Events</span></span>                      | <span data-ttu-id="bdcee-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bdcee-116">Calendars.Read</span></span>      |
| <span data-ttu-id="bdcee-117">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="bdcee-117">Messages</span></span>                    | <span data-ttu-id="bdcee-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bdcee-118">Mail.Read</span></span>           |
| <span data-ttu-id="bdcee-119">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="bdcee-119">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="bdcee-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bdcee-120">Files.ReadWrite</span></span>     |
| <span data-ttu-id="bdcee-121">Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="bdcee-121">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="bdcee-122">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdcee-122">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdcee-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdcee-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /subscriptions/{subscriptionId}
```

## <a name="request-headers"></a><span data-ttu-id="bdcee-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bdcee-124">Request headers</span></span>
| <span data-ttu-id="bdcee-125">Name</span><span class="sxs-lookup"><span data-stu-id="bdcee-125">Name</span></span>       | <span data-ttu-id="bdcee-126">Typ</span><span class="sxs-lookup"><span data-stu-id="bdcee-126">Type</span></span> | <span data-ttu-id="bdcee-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdcee-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bdcee-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdcee-128">Authorization</span></span>  | <span data-ttu-id="bdcee-129">string</span><span class="sxs-lookup"><span data-stu-id="bdcee-129">string</span></span>  | <span data-ttu-id="bdcee-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bdcee-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bdcee-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdcee-132">Response</span></span>

<span data-ttu-id="bdcee-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bdcee-133">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bdcee-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bdcee-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdcee-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bdcee-135">Request</span></span>
<span data-ttu-id="bdcee-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bdcee-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="bdcee-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="bdcee-137">Response</span></span>
<span data-ttu-id="bdcee-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bdcee-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
