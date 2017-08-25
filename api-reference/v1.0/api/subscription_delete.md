# <a name="delete-subscription"></a><span data-ttu-id="6b462-101">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="6b462-101">Delete subscription</span></span>

<span data-ttu-id="6b462-102">Mit dieser API können Sie Abonnements löschen.</span><span class="sxs-lookup"><span data-stu-id="6b462-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b462-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6b462-103">Permissions</span></span>

<span data-ttu-id="6b462-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b462-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="6b462-106">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="6b462-106">Resource type / Item</span></span>        | <span data-ttu-id="6b462-107">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="6b462-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="6b462-108">Kontakte</span><span class="sxs-lookup"><span data-stu-id="6b462-108">Contacts</span></span>                    | <span data-ttu-id="6b462-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6b462-109">Contacts.Read</span></span>       |
| <span data-ttu-id="6b462-110">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="6b462-110">Conversations</span></span>               | <span data-ttu-id="6b462-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b462-111">Group.Read.All</span></span>      |
| <span data-ttu-id="6b462-112">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="6b462-112">Events</span></span>                      | <span data-ttu-id="6b462-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6b462-113">Calendars.Read</span></span>      |
| <span data-ttu-id="6b462-114">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="6b462-114">Messages</span></span>                    | <span data-ttu-id="6b462-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6b462-115">Mail.Read</span></span>           |
| <span data-ttu-id="6b462-116">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="6b462-116">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="6b462-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b462-117">Files.ReadWrite</span></span>     |
| <span data-ttu-id="6b462-118">Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="6b462-118">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="6b462-119">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b462-119">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b462-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b462-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a><span data-ttu-id="6b462-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b462-121">Request headers</span></span>
| <span data-ttu-id="6b462-122">Name</span><span class="sxs-lookup"><span data-stu-id="6b462-122">Name</span></span>       | <span data-ttu-id="6b462-123">Typ</span><span class="sxs-lookup"><span data-stu-id="6b462-123">Type</span></span> | <span data-ttu-id="6b462-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b462-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6b462-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b462-125">Authorization</span></span>  | <span data-ttu-id="6b462-126">string</span><span class="sxs-lookup"><span data-stu-id="6b462-126">string</span></span>  | <span data-ttu-id="6b462-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6b462-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b462-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b462-129">Request body</span></span>
<span data-ttu-id="6b462-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6b462-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b462-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b462-131">Response</span></span>

<span data-ttu-id="6b462-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b462-132">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="6b462-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b462-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b462-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b462-134">Request</span></span>
<span data-ttu-id="6b462-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b462-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="6b462-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b462-136">Response</span></span>
<span data-ttu-id="6b462-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6b462-137">Here is an example of the response.</span></span>
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
