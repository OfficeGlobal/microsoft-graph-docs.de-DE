# <a name="delete-attachment"></a><span data-ttu-id="6deb8-101">Anlage löschen</span><span class="sxs-lookup"><span data-stu-id="6deb8-101">Delete attachment</span></span>

<span data-ttu-id="6deb8-102">Mit dieser API können Sie Anlagen aus Kalenderereignissen, E-Mail-Nachrichten oder Gruppenbeiträgen löschen.</span><span class="sxs-lookup"><span data-stu-id="6deb8-102">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="6deb8-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6deb8-103">Permissions</span></span>
<span data-ttu-id="6deb8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6deb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="6deb8-106">Beim Zugriff auf Anlagen in Nachrichten: Mail.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="6deb8-106">If accessing attachments in Messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="6deb8-107">Beim Zugriff auf Anlagen in Ereignissen: Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="6deb8-107">If accessing attachments in Events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="6deb8-108">Beim Zugriff auf Anlagen in Gruppenbeiträgen: Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="6deb8-108">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="6deb8-109">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6deb8-109">HTTP request</span></span>
<span data-ttu-id="6deb8-110">Anlagen für ein [Ereignis](../resources/event.md) im Standard[kalender](../resources/calendar.md) des Benutzers oder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="6deb8-110">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="6deb8-111">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der standardmäßigen [calendarGroup](../resources/calendargroup.md) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="6deb8-111">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="6deb8-112">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="6deb8-112">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="6deb8-113">Anlagen für eine [Nachricht](../resources/message.md) im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="6deb8-113">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="6deb8-114">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="6deb8-114">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="6deb8-115">Anlagen für eine [Nachricht](../resources/message.md) in einem untergeordneten Ordner eines [mailFolder](../resources/mailfolder.md) im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="6deb8-115">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="6deb8-116">Das folgende Beispiel zeigt eine Ebene der Verschachtelung. Eine Nachricht kann jedoch auch in einem untergeordneten Ordner eines untergeordneten Ordners und so weiter enthalten sein.</span><span class="sxs-lookup"><span data-stu-id="6deb8-116">A contact contained in a child folder of a contactFolder. The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="6deb8-117">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="6deb8-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6deb8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6deb8-118">Request headers</span></span>
| <span data-ttu-id="6deb8-119">Name</span><span class="sxs-lookup"><span data-stu-id="6deb8-119">Name</span></span>       | <span data-ttu-id="6deb8-120">Typ</span><span class="sxs-lookup"><span data-stu-id="6deb8-120">Type</span></span> | <span data-ttu-id="6deb8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6deb8-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6deb8-122">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6deb8-122">Authorization</span></span>  | <span data-ttu-id="6deb8-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6deb8-123">string</span></span>  | <span data-ttu-id="6deb8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6deb8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6deb8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6deb8-126">Request body</span></span>
<span data-ttu-id="6deb8-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6deb8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6deb8-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="6deb8-128">Response</span></span>

<span data-ttu-id="6deb8-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6deb8-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6deb8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6deb8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6deb8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6deb8-132">Request</span></span>
<span data-ttu-id="6deb8-133">Hier finden Sie ein Beispiel für die Anforderung zum Löschen einer Anlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="6deb8-133">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="6deb8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6deb8-134">Response</span></span>
<span data-ttu-id="6deb8-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6deb8-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
