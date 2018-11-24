# <a name="delete-subscription"></a><span data-ttu-id="68cd2-101">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="68cd2-101">Delete subscription</span></span>

<span data-ttu-id="68cd2-102">Mit dieser API können Sie Abonnements löschen.</span><span class="sxs-lookup"><span data-stu-id="68cd2-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="68cd2-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="68cd2-103">Permissions</span></span>

<span data-ttu-id="68cd2-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="68cd2-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="68cd2-106">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="68cd2-106">Resource type / Item</span></span>        | <span data-ttu-id="68cd2-107">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="68cd2-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="68cd2-108">Kontakte</span><span class="sxs-lookup"><span data-stu-id="68cd2-108">Contacts</span></span>                    | <span data-ttu-id="68cd2-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="68cd2-109">Contacts.Read</span></span>       |
| <span data-ttu-id="68cd2-110">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="68cd2-110">Conversations</span></span>               | <span data-ttu-id="68cd2-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="68cd2-111">Group.Read.All</span></span>      |
| <span data-ttu-id="68cd2-112">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="68cd2-112">Events</span></span>                      | <span data-ttu-id="68cd2-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="68cd2-113">Calendars.Read</span></span>      |
| <span data-ttu-id="68cd2-114">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="68cd2-114">Messages</span></span>                    | <span data-ttu-id="68cd2-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="68cd2-115">Mail.Read</span></span>           |
| <span data-ttu-id="68cd2-116">Gruppen</span><span class="sxs-lookup"><span data-stu-id="68cd2-116">Groups</span></span>                      | <span data-ttu-id="68cd2-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="68cd2-117">Group.Read.All</span></span>      |
| <span data-ttu-id="68cd2-118">Benutzer</span><span class="sxs-lookup"><span data-stu-id="68cd2-118">Users</span></span>                       | <span data-ttu-id="68cd2-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="68cd2-119">User.Read.All</span></span>       |
| <span data-ttu-id="68cd2-120">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="68cd2-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="68cd2-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68cd2-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="68cd2-122">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="68cd2-122">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="68cd2-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cd2-123">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="68cd2-124">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="68cd2-124">Security alert</span></span>| <span data-ttu-id="68cd2-125">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cd2-125">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68cd2-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="68cd2-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="68cd2-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="68cd2-127">Request headers</span></span>

| <span data-ttu-id="68cd2-128">Name</span><span class="sxs-lookup"><span data-stu-id="68cd2-128">Name</span></span>       | <span data-ttu-id="68cd2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="68cd2-129">Type</span></span> | <span data-ttu-id="68cd2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68cd2-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="68cd2-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="68cd2-131">Authorization</span></span>  | <span data-ttu-id="68cd2-132">string</span><span class="sxs-lookup"><span data-stu-id="68cd2-132">string</span></span>  | <span data-ttu-id="68cd2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="68cd2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68cd2-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="68cd2-135">Request body</span></span>

<span data-ttu-id="68cd2-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="68cd2-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68cd2-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="68cd2-137">Response</span></span>

<span data-ttu-id="68cd2-138">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68cd2-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="68cd2-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="68cd2-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="68cd2-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="68cd2-140">Request</span></span>

<span data-ttu-id="68cd2-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68cd2-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="68cd2-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="68cd2-142">Response</span></span>

<span data-ttu-id="68cd2-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="68cd2-143">Here is an example of the response.</span></span>
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
