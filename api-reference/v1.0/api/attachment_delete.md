# <a name="delete-attachment"></a><span data-ttu-id="2f6b5-101">Anlage löschen</span><span class="sxs-lookup"><span data-stu-id="2f6b5-101">Delete attachment</span></span>

<span data-ttu-id="2f6b5-102">Mit dieser API können Sie Anlagen aus Kalenderereignissen, E-Mail-Nachrichten oder Gruppenbeiträgen löschen.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-102">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f6b5-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2f6b5-103">Permissions</span></span>
<span data-ttu-id="2f6b5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f6b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="2f6b5-106">Beim Zugriff auf Anlagen in Nachrichten: Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f6b5-106">If accessing attachments in Messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="2f6b5-107">Beim Zugriff auf Anlagen in Ereignissen: Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f6b5-107">If accessing attachments in Events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="2f6b5-108">Beim Zugriff auf Anlagen in Gruppenereignissen oder -beiträgen: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f6b5-108">If accessing attachments in Group Events or Posts: Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="2f6b5-109">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f6b5-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="2f6b5-110">Anlagen für ein [Ereignis](../resources/event.md) im Standard[kalender](../resources/calendar.md) des Benutzers oder der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-110">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
DELETE /groups/{id}/events/{id}/attachments/{id}

DELETE /me/calendar/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
```
<span data-ttu-id="2f6b5-111">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der standardmäßigen [calendarGroup](../resources/calendargroup.md) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-111">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="2f6b5-112">Anlagen für ein [Ereignis](../resources/event.md) in einem [Kalender](../resources/calendar.md) aus der [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-112">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="2f6b5-113">Anlagen für eine [Nachricht](../resources/message.md) im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-113">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="2f6b5-114">Anlagen für eine [Nachricht](../resources/message.md) in einem [MailFolder](../resources/mailfolder.md) der obersten Ebene im Postfach eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-114">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="2f6b5-p102">Anlagen für eine [Nachricht](../resources/message.md) in einem untergeordneten [MailFolder](../resources/mailfolder.md) im Postfach eines Benutzers.  Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber eine Nachricht kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="2f6b5-117">Anlagen für einen [Beitrag](../resources/post.md) in einem [Thread](../resources/conversationthread.md), der zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2f6b5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2f6b5-118">Request headers</span></span>
| <span data-ttu-id="2f6b5-119">Name</span><span class="sxs-lookup"><span data-stu-id="2f6b5-119">Name</span></span>       | <span data-ttu-id="2f6b5-120">Typ</span><span class="sxs-lookup"><span data-stu-id="2f6b5-120">Type</span></span> | <span data-ttu-id="2f6b5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2f6b5-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f6b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f6b5-122">Authorization</span></span>  | <span data-ttu-id="2f6b5-123">string</span><span class="sxs-lookup"><span data-stu-id="2f6b5-123">string</span></span>  | <span data-ttu-id="2f6b5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f6b5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2f6b5-126">Request body</span></span>
<span data-ttu-id="2f6b5-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f6b5-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f6b5-128">Response</span></span>

<span data-ttu-id="2f6b5-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f6b5-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2f6b5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f6b5-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2f6b5-132">Request</span></span>
<span data-ttu-id="2f6b5-133">Hier finden Sie ein Beispiel für die Anforderung zum Löschen einer Anlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-133">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="2f6b5-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2f6b5-134">Response</span></span>
<span data-ttu-id="2f6b5-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2f6b5-135">Here is an example of the response.</span></span>
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
