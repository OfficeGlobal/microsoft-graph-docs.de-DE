---
title: Abonnement erstellen
description: Diese API abonniert eine Listeneranwendung, über die sie Benachrichtigungen erhält, sobald Daten in Microsoft Graph geändert werden.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 6d06e230dd85aadaa4d2b3a4f851b339b34793eb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157694"
---
# <a name="create-subscription"></a><span data-ttu-id="ae6ff-103">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="ae6ff-103">Create subscription</span></span>

<span data-ttu-id="ae6ff-104">Abonniert eine Listener-Anwendung, um Benachrichtigungen zu erhalten, wenn die angeforderte Art von Änderungen an der angegebenen Ressource in Microsoft Graph auftritt.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae6ff-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ae6ff-105">Permissions</span></span>

 <span data-ttu-id="ae6ff-106">Zur Abonnementerstellung ist Lesezugriff auf die Ressource erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-106">Creating a subscription requires read scope to the resource; e.g.  is required to get notifications on Inbox messages.</span></span> <span data-ttu-id="ae6ff-107">Beispiel: um Benachrichtigungen zu Nachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="ae6ff-108">Abhängig von der Ressource und dem angeforderten Berechtigungstyp (delegiert oder Anwendung) ist die in der folgenden Tabelle angegebene Berechtigung die niedrigste Berechtigung, die zum Aufrufen dieser API erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="ae6ff-109">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae6ff-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae6ff-110">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="ae6ff-110">Supported resource</span></span> | <span data-ttu-id="ae6ff-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae6ff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae6ff-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae6ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae6ff-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae6ff-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="ae6ff-114">contact</span><span class="sxs-lookup"><span data-stu-id="ae6ff-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="ae6ff-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ae6ff-115">Contacts.Read</span></span> | <span data-ttu-id="ae6ff-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ae6ff-116">Contacts.Read</span></span> | <span data-ttu-id="ae6ff-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ae6ff-117">Contacts.Read</span></span> |
|<span data-ttu-id="ae6ff-118">[driveItem](../resources/driveitem.md) (persönliche OneDrive-Umgebung eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="ae6ff-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="ae6ff-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae6ff-119">Not supported</span></span> | <span data-ttu-id="ae6ff-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae6ff-120">Files.ReadWrite</span></span> | <span data-ttu-id="ae6ff-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae6ff-121">Not supported</span></span> |
|<span data-ttu-id="ae6ff-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="ae6ff-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="ae6ff-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae6ff-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="ae6ff-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae6ff-124">Not supported</span></span> | <span data-ttu-id="ae6ff-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae6ff-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="ae6ff-126">event</span><span class="sxs-lookup"><span data-stu-id="ae6ff-126">event</span></span>](../resources/event.md) | <span data-ttu-id="ae6ff-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae6ff-127">Calendars.Read</span></span> | <span data-ttu-id="ae6ff-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae6ff-128">Calendars.Read</span></span> | <span data-ttu-id="ae6ff-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ae6ff-129">Calendars.Read</span></span> |
|[<span data-ttu-id="ae6ff-130">group</span><span class="sxs-lookup"><span data-stu-id="ae6ff-130">group</span></span>](../resources/group.md) | <span data-ttu-id="ae6ff-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae6ff-131">Group.Read.All</span></span> | <span data-ttu-id="ae6ff-132">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae6ff-132">Not supported</span></span> | <span data-ttu-id="ae6ff-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae6ff-133">Group.Read.All</span></span> |
|[<span data-ttu-id="ae6ff-134">group conversation</span><span class="sxs-lookup"><span data-stu-id="ae6ff-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="ae6ff-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae6ff-135">Group.Read.All</span></span> | <span data-ttu-id="ae6ff-136">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae6ff-136">Not supported</span></span> | <span data-ttu-id="ae6ff-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae6ff-137">Not supported</span></span> |
|[<span data-ttu-id="ae6ff-138">message</span><span class="sxs-lookup"><span data-stu-id="ae6ff-138">message</span></span>](../resources/message.md) | <span data-ttu-id="ae6ff-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ae6ff-139">Mail.Read</span></span> | <span data-ttu-id="ae6ff-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ae6ff-140">Mail.Read</span></span> | <span data-ttu-id="ae6ff-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ae6ff-141">Mail.Read</span></span> |
|[<span data-ttu-id="ae6ff-142">security alert</span><span class="sxs-lookup"><span data-stu-id="ae6ff-142">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="ae6ff-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae6ff-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="ae6ff-144">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae6ff-144">Not supported</span></span> | <span data-ttu-id="ae6ff-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae6ff-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="ae6ff-146">user</span><span class="sxs-lookup"><span data-stu-id="ae6ff-146">user</span></span>](../resources/user.md) | <span data-ttu-id="ae6ff-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae6ff-147">User.Read.All</span></span> | <span data-ttu-id="ae6ff-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae6ff-148">User.Read.All</span></span> | <span data-ttu-id="ae6ff-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae6ff-149">User.Read.All</span></span> |

> <span data-ttu-id="ae6ff-150">**Hinweis:** Es gibt zusätzliche Einschränkungen für Abonnements für OneDrive- und Outlook-Elemente.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="ae6ff-151">Die Einschränkungen gelten sowohl für die Erstellung als auch für die Verwaltung von Abonnements (Abrufen, Aktualisieren und Löschen von Abonnements).</span><span class="sxs-lookup"><span data-stu-id="ae6ff-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="ae6ff-152">Auf dem persönlichen OneDrive können Sie den Stammordner oder einen beliebigen Unterordner auf diesem Laufwerk abonnieren.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="ae6ff-153">Bei OneDrive for Business können Sie nur den Stammordner abonnieren.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="ae6ff-154">Benachrichtigungen werden für die angeforderten Arten von Änderungen am abonnierten Ordner bzw. an einer Datei, einem Ordner oder anderen **driveItem**-Instanzen in seiner Hierarchie gesendet.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="ae6ff-155">Sie können keine **drive**- oder **driveItem**-Instanzen abonnieren, die keine Ordner sind, wie beispielsweise einzelne Dateien.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="ae6ff-156">In Outlook unterstützt die delegierte Berechtigung das Abonnieren von Elementen ausschließlich in Ordnern, die sich im Postfach des angemeldeten Benutzers befinden.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="ae6ff-157">Das bedeutet, dass Sie beispielsweise nicht die delegierte Berechtigung "Calendars.Read" verwenden können, um Ereignisse im Postfach eines anderen Benutzers zu abonnieren.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="ae6ff-158">So abonnieren Sie Änderungsbenachrichtigungen über Outlook-Kontakte, -Ereignisse oder -Nachrichten in _freigegebenen oder delegierten Ordnern_:</span><span class="sxs-lookup"><span data-stu-id="ae6ff-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="ae6ff-159">Verwenden Sie die entsprechende Anwendungsberechtigung, um Änderungen von Elementen in einem Ordner oder Postfach eines _beliebigen_ Benutzers im Mandanten zu abonnieren.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="ae6ff-160">Verwenden Sie nicht die Outlook-Freigabeberechtigungen (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared und ihre read/write-Entsprechungen), da sie **nicht** das Abonnieren von Änderungsbenachrichtigungen für Elemente in freigegebenen oder delegierten Ordnern unterstützen.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span> 


## <a name="http-request"></a><span data-ttu-id="ae6ff-161">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae6ff-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="ae6ff-162">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae6ff-162">Request headers</span></span>

| <span data-ttu-id="ae6ff-163">Name</span><span class="sxs-lookup"><span data-stu-id="ae6ff-163">Name</span></span>       | <span data-ttu-id="ae6ff-164">Typ</span><span class="sxs-lookup"><span data-stu-id="ae6ff-164">Type</span></span> | <span data-ttu-id="ae6ff-165">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae6ff-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ae6ff-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae6ff-166">Authorization</span></span>  | <span data-ttu-id="ae6ff-167">string</span><span class="sxs-lookup"><span data-stu-id="ae6ff-167">string</span></span>  | <span data-ttu-id="ae6ff-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ae6ff-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae6ff-170">Response</span></span>

<span data-ttu-id="ae6ff-171">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae6ff-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae6ff-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ae6ff-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae6ff-173">Request</span></span>

<span data-ttu-id="ae6ff-174">Hier sehen Sie ein Beispiel für die Anforderung zum Senden einer Benachrichtigung, wenn der Benutzer eine neue E-Mail empfängt.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-174">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="ae6ff-175">Geben Sie im Anforderungstext eine JSON-Darstellung des [subscription](../resources/subscription.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-175">In the request body, supply a JSON representation of the [onlineMeeting](../resources/subscription.md) object.</span></span>
<span data-ttu-id="ae6ff-176">Das `clientState`-Feld ist optional.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-176">The `clientState` parameter is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="ae6ff-177">Beispiele für Ressourcen</span><span class="sxs-lookup"><span data-stu-id="ae6ff-177">Resources examples</span></span>

<span data-ttu-id="ae6ff-178">Im Folgenden sind gültige Werte für die Ressourceneigenschaft des Abonnements aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="ae6ff-178">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="ae6ff-179">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ae6ff-179">Resource type</span></span> | <span data-ttu-id="ae6ff-180">Beispiele</span><span class="sxs-lookup"><span data-stu-id="ae6ff-180">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="ae6ff-181">Mail</span><span class="sxs-lookup"><span data-stu-id="ae6ff-181">Mail</span></span>|<span data-ttu-id="ae6ff-182">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="ae6ff-182">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="ae6ff-183">me/messages</span><span class="sxs-lookup"><span data-stu-id="ae6ff-183">me/messages</span></span>|
|<span data-ttu-id="ae6ff-184">Kontakte</span><span class="sxs-lookup"><span data-stu-id="ae6ff-184">Contacts</span></span>|<span data-ttu-id="ae6ff-185">me/contacts</span><span class="sxs-lookup"><span data-stu-id="ae6ff-185">me/contacts</span></span>|
|<span data-ttu-id="ae6ff-186">Kalender</span><span class="sxs-lookup"><span data-stu-id="ae6ff-186">Calendars</span></span>|<span data-ttu-id="ae6ff-187">me/events</span><span class="sxs-lookup"><span data-stu-id="ae6ff-187">me/events</span></span>|
|<span data-ttu-id="ae6ff-188">Benutzer</span><span class="sxs-lookup"><span data-stu-id="ae6ff-188">Users</span></span>|<span data-ttu-id="ae6ff-189">users</span><span class="sxs-lookup"><span data-stu-id="ae6ff-189">users</span></span>|
|<span data-ttu-id="ae6ff-190">Gruppen</span><span class="sxs-lookup"><span data-stu-id="ae6ff-190">Groups</span></span>|<span data-ttu-id="ae6ff-191">groups</span><span class="sxs-lookup"><span data-stu-id="ae6ff-191">groups</span></span>|
|<span data-ttu-id="ae6ff-192">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="ae6ff-192">Conversations</span></span>|<span data-ttu-id="ae6ff-193">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="ae6ff-193">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="ae6ff-194">Laufwerke</span><span class="sxs-lookup"><span data-stu-id="ae6ff-194">Drives</span></span>|<span data-ttu-id="ae6ff-195">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="ae6ff-195">me/drive/root</span></span>|
|<span data-ttu-id="ae6ff-196">Sicherheitswarnung</span><span class="sxs-lookup"><span data-stu-id="ae6ff-196">Security alert</span></span>|<span data-ttu-id="ae6ff-197">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="ae6ff-197">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="ae6ff-198">Reaktion</span><span class="sxs-lookup"><span data-stu-id="ae6ff-198">Response</span></span>

<span data-ttu-id="ae6ff-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="ae6ff-202">Endpunktprüfung für Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="ae6ff-202">Notification endpoint validation</span></span>

<span data-ttu-id="ae6ff-203">Der Endpunkt der Abonnementbenachrichtigung (angegeben in der Eigenschaft `notificationUrl`) muss in der Lage sein, auf eine Validierungsanforderung zu reagieren, wie unter [Einrichten von Benachrichtigungen für Änderungen an Benutzerdaten](/graph/webhooks#notification-endpoint-validation) beschrieben.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-203">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="ae6ff-204">Wenn die Validierung fehlschlägt, gibt die Anforderung zur Erstellung des Abonnements einen "400 Bad Request"-Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="ae6ff-204">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
