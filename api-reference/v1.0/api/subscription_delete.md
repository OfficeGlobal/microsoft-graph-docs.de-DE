# <a name="delete-subscription"></a><span data-ttu-id="409e5-101">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="409e5-101">Delete subscription</span></span>

<span data-ttu-id="409e5-102">Mit dieser API können Sie Abonnements löschen.</span><span class="sxs-lookup"><span data-stu-id="409e5-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="409e5-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="409e5-103">Permissions</span></span>

<span data-ttu-id="409e5-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="409e5-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="409e5-106">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="409e5-106">Resource type / Item</span></span>        | <span data-ttu-id="409e5-107">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="409e5-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="409e5-108">Kontakte</span><span class="sxs-lookup"><span data-stu-id="409e5-108">Contacts</span></span>                    | <span data-ttu-id="409e5-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="409e5-109">Contacts.Read</span></span>       |
| <span data-ttu-id="409e5-110">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="409e5-110">Conversations</span></span>               | <span data-ttu-id="409e5-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="409e5-111">Group.Read.All</span></span>      |
| <span data-ttu-id="409e5-112">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="409e5-112">Events</span></span>                      | <span data-ttu-id="409e5-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="409e5-113">Calendars.Read</span></span>      |
| <span data-ttu-id="409e5-114">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="409e5-114">Messages</span></span>                    | <span data-ttu-id="409e5-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="409e5-115">Mail.Read</span></span>           |
| <span data-ttu-id="409e5-116">Gruppen</span><span class="sxs-lookup"><span data-stu-id="409e5-116">Groups</span></span>                      | <span data-ttu-id="409e5-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="409e5-117">Group.Read.All</span></span>      |
| <span data-ttu-id="409e5-118">Benutzer</span><span class="sxs-lookup"><span data-stu-id="409e5-118">Users</span></span>                       | <span data-ttu-id="409e5-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="409e5-119">User.Read.All</span></span>       |
| <span data-ttu-id="409e5-120">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="409e5-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="409e5-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="409e5-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="409e5-122">Laufwerke (freigegebene SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="409e5-122">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="409e5-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="409e5-123">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="409e5-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="409e5-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="409e5-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="409e5-125">Request headers</span></span>

| <span data-ttu-id="409e5-126">Name</span><span class="sxs-lookup"><span data-stu-id="409e5-126">Name</span></span>       | <span data-ttu-id="409e5-127">Typ</span><span class="sxs-lookup"><span data-stu-id="409e5-127">Type</span></span> | <span data-ttu-id="409e5-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="409e5-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="409e5-129">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="409e5-129">Authorization</span></span>  | <span data-ttu-id="409e5-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="409e5-130">string</span></span>  | <span data-ttu-id="409e5-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="409e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="409e5-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="409e5-133">Request body</span></span>

<span data-ttu-id="409e5-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="409e5-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="409e5-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="409e5-135">Response</span></span>

<span data-ttu-id="409e5-136">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="409e5-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="409e5-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="409e5-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="409e5-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="409e5-138">Request</span></span>

<span data-ttu-id="409e5-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="409e5-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="409e5-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="409e5-140">Response</span></span>

<span data-ttu-id="409e5-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="409e5-141">Here is an example of the response.</span></span>
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
