---
title: Abonnement erstellen
description: Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Daten in einer Microsoft Graph-Ressource geändert werden.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: a8b8189780ac0b820551fb885adcf843c9ebe8f4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140166"
---
# <a name="create-subscription"></a><span data-ttu-id="beba6-103">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="beba6-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beba6-104">Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn der angeforderte Änderungstyp für die angegebene Ressource in Microsoft Graph auftritt.</span><span class="sxs-lookup"><span data-stu-id="beba6-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="beba6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="beba6-105">Permissions</span></span>

<span data-ttu-id="beba6-106">Das Erstellen eines Abonnements erfordert Lesebereich für die Ressource.</span><span class="sxs-lookup"><span data-stu-id="beba6-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="beba6-107">Wenn Sie beispielsweise Benachrichtigungen zu Nachrichten erhalten möchten, benötigt Ihre `Mail.Read` APP die Berechtigung.</span><span class="sxs-lookup"><span data-stu-id="beba6-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="beba6-108">Abhängig von der angeforderten Ressource und dem Berechtigungstyp (Delegierte oder Anwendung) ist die in der folgenden Tabelle angegebene Berechtigung die am wenigsten privilegierten Berechtigungen zum Aufrufen dieser API.</span><span class="sxs-lookup"><span data-stu-id="beba6-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="beba6-109">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beba6-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="beba6-110">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="beba6-110">Supported resource</span></span> | <span data-ttu-id="beba6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="beba6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="beba6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="beba6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beba6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="beba6-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="beba6-114">Kontakt</span><span class="sxs-lookup"><span data-stu-id="beba6-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="beba6-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="beba6-115">Contacts.Read</span></span> | <span data-ttu-id="beba6-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="beba6-116">Contacts.Read</span></span> | <span data-ttu-id="beba6-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="beba6-117">Contacts.Read</span></span> |
|<span data-ttu-id="beba6-118">[driveItem](../resources/driveitem.md) (persönliche OneDrive des Benutzers)</span><span class="sxs-lookup"><span data-stu-id="beba6-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="beba6-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beba6-119">Not supported</span></span> | <span data-ttu-id="beba6-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="beba6-120">Files.ReadWrite</span></span> | <span data-ttu-id="beba6-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beba6-121">Not supported</span></span> |
|<span data-ttu-id="beba6-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="beba6-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="beba6-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beba6-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="beba6-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beba6-124">Not supported</span></span> | <span data-ttu-id="beba6-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beba6-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="beba6-126">event</span><span class="sxs-lookup"><span data-stu-id="beba6-126">event</span></span>](../resources/event.md) | <span data-ttu-id="beba6-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="beba6-127">Calendars.Read</span></span> | <span data-ttu-id="beba6-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="beba6-128">Calendars.Read</span></span> | <span data-ttu-id="beba6-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="beba6-129">Calendars.Read</span></span> |
|[<span data-ttu-id="beba6-130">group</span><span class="sxs-lookup"><span data-stu-id="beba6-130">group</span></span>](../resources/group.md) | <span data-ttu-id="beba6-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="beba6-131">Group.Read.All</span></span> | <span data-ttu-id="beba6-132">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beba6-132">Not supported</span></span> | <span data-ttu-id="beba6-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="beba6-133">Group.Read.All</span></span> |
|[<span data-ttu-id="beba6-134">Gruppenunterhaltung</span><span class="sxs-lookup"><span data-stu-id="beba6-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="beba6-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="beba6-135">Group.Read.All</span></span> | <span data-ttu-id="beba6-136">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beba6-136">Not supported</span></span> | <span data-ttu-id="beba6-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beba6-137">Not supported</span></span> |
|[<span data-ttu-id="beba6-138">Nachricht</span><span class="sxs-lookup"><span data-stu-id="beba6-138">message</span></span>](../resources/message.md) | <span data-ttu-id="beba6-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="beba6-139">Mail.Read</span></span> | <span data-ttu-id="beba6-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="beba6-140">Mail.Read</span></span> | <span data-ttu-id="beba6-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="beba6-141">Mail.Read</span></span> |
|[<span data-ttu-id="beba6-142">Sicherheitswarnung</span><span class="sxs-lookup"><span data-stu-id="beba6-142">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="beba6-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beba6-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="beba6-144">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beba6-144">Not supported</span></span> | <span data-ttu-id="beba6-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beba6-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="beba6-146">user</span><span class="sxs-lookup"><span data-stu-id="beba6-146">user</span></span>](../resources/user.md) | <span data-ttu-id="beba6-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="beba6-147">User.Read.All</span></span> | <span data-ttu-id="beba6-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="beba6-148">User.Read.All</span></span> | <span data-ttu-id="beba6-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="beba6-149">User.Read.All</span></span> |

> <span data-ttu-id="beba6-150">**Hinweis:** Es gibt zusätzliche Einschränkungen für Abonnements für OneDrive-und Outlook-Elemente.</span><span class="sxs-lookup"><span data-stu-id="beba6-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="beba6-151">Die Einschränkungen gelten für das Erstellen und Verwalten von Abonnements (erhalten, aktualisieren und Löschen von Abonnements).</span><span class="sxs-lookup"><span data-stu-id="beba6-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="beba6-152">In persönlichen OneDrive können Sie den Stammordner oder einen beliebigen Unterordner in diesem Laufwerk abonnieren.</span><span class="sxs-lookup"><span data-stu-id="beba6-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="beba6-153">In OneDrive for Business können Sie nur den Stammordner abonnieren.</span><span class="sxs-lookup"><span data-stu-id="beba6-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="beba6-154">Benachrichtigungen werden für die angeforderten Änderungstypen im abonnierten Ordner oder für eine beliebige Datei, einen Ordner oder eine andere **driveItem** -Instanz in der Hierarchie gesendet.</span><span class="sxs-lookup"><span data-stu-id="beba6-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="beba6-155">Sie können keine **Laufwerks** -oder **driveItem** -Instanzen abonnieren, die keine Ordner sind, wie beispielsweise einzelne Dateien.</span><span class="sxs-lookup"><span data-stu-id="beba6-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="beba6-156">In Outlook unterstützt die Delegierte Berechtigung das Abonnieren von Elementen in Ordnern nur im Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="beba6-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="beba6-157">Das kann beispielsweise nicht die Delegierte Berechtigung Calendars. Read verwenden, um Ereignisse im Postfach eines anderen Benutzers zu abonnieren.</span><span class="sxs-lookup"><span data-stu-id="beba6-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="beba6-158">So abonnieren Sie Änderungsbenachrichtigungen für Outlook-Kontakte,-Ereignisse oder-Nachrichten in _freigegebenen oder Delegierten_ Ordnern:</span><span class="sxs-lookup"><span data-stu-id="beba6-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="beba6-159">Verwenden Sie die entsprechende Anwendungsberechtigung, um Änderungen an Elementen in einem Ordner oder Postfach eines _beliebigen_ Benutzers im Mandanten zu abonnieren.</span><span class="sxs-lookup"><span data-stu-id="beba6-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="beba6-160">Verwenden Sie nicht die Outlook-Freigabeberechtigungen (Contacts. Read. Shared, Calendars. Read. Shared, Mail. Read. Shared und ihre Pendants für Lese-/Schreibzugriff), da Sie das Abonnieren von Änderungsbenachrichtigungen für Elemente in freigegebenen oder Delegierten Ordnern **nicht** unterstützen.</span><span class="sxs-lookup"><span data-stu-id="beba6-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="beba6-161">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="beba6-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="beba6-162">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="beba6-162">Request headers</span></span>

| <span data-ttu-id="beba6-163">Name</span><span class="sxs-lookup"><span data-stu-id="beba6-163">Name</span></span>       | <span data-ttu-id="beba6-164">Typ</span><span class="sxs-lookup"><span data-stu-id="beba6-164">Type</span></span> | <span data-ttu-id="beba6-165">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="beba6-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="beba6-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="beba6-166">Authorization</span></span>  | <span data-ttu-id="beba6-167">string</span><span class="sxs-lookup"><span data-stu-id="beba6-167">string</span></span>  | <span data-ttu-id="beba6-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="beba6-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="beba6-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="beba6-170">Response</span></span>

<span data-ttu-id="beba6-171">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="beba6-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beba6-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="beba6-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="beba6-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="beba6-173">Request</span></span>

<span data-ttu-id="beba6-174">Geben Sie im Anforderungstext eine JSON-Darstellung des [Subscription](../resources/subscription.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="beba6-174">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="beba6-175">Das `clientState` Feld ist optional.</span><span class="sxs-lookup"><span data-stu-id="beba6-175">The `clientState` field is optional.</span></span>

<span data-ttu-id="beba6-176">In dieser Beispielanforderung wird ein Abonnement für Benachrichtigungen über neue e-Mails erstellt, die von dem derzeit signierten Benutzer empfangen werden.</span><span class="sxs-lookup"><span data-stu-id="beba6-176">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="beba6-177">Die folgenden Werte gelten für die Resource-Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="beba6-177">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="beba6-178">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="beba6-178">Resource type</span></span> | <span data-ttu-id="beba6-179">Beispiele</span><span class="sxs-lookup"><span data-stu-id="beba6-179">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="beba6-180">Mail</span><span class="sxs-lookup"><span data-stu-id="beba6-180">Mail</span></span>|<span data-ttu-id="beba6-181">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="beba6-181">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="beba6-182">me/messages</span><span class="sxs-lookup"><span data-stu-id="beba6-182">me/messages</span></span>|
|<span data-ttu-id="beba6-183">Kontakte</span><span class="sxs-lookup"><span data-stu-id="beba6-183">Contacts</span></span>|<span data-ttu-id="beba6-184">me/contacts</span><span class="sxs-lookup"><span data-stu-id="beba6-184">me/contacts</span></span>|
|<span data-ttu-id="beba6-185">Kalender</span><span class="sxs-lookup"><span data-stu-id="beba6-185">Calendars</span></span>|<span data-ttu-id="beba6-186">me/events</span><span class="sxs-lookup"><span data-stu-id="beba6-186">me/events</span></span>|
|<span data-ttu-id="beba6-187">Benutzer</span><span class="sxs-lookup"><span data-stu-id="beba6-187">Users</span></span>|<span data-ttu-id="beba6-188">users</span><span class="sxs-lookup"><span data-stu-id="beba6-188">users</span></span>|
|<span data-ttu-id="beba6-189">Gruppen</span><span class="sxs-lookup"><span data-stu-id="beba6-189">Groups</span></span>|<span data-ttu-id="beba6-190">Gruppen</span><span class="sxs-lookup"><span data-stu-id="beba6-190">groups</span></span>|
|<span data-ttu-id="beba6-191">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="beba6-191">Conversations</span></span>|<span data-ttu-id="beba6-192">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="beba6-192">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="beba6-193">Laufwerke</span><span class="sxs-lookup"><span data-stu-id="beba6-193">Drives</span></span>|<span data-ttu-id="beba6-194">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="beba6-194">me/drive/root</span></span>|
|<span data-ttu-id="beba6-195">Sicherheitswarnung</span><span class="sxs-lookup"><span data-stu-id="beba6-195">Security alert</span></span>|<span data-ttu-id="beba6-196">Sicherheit/Warnungen? $filter = Status-EQ ' neu '</span><span class="sxs-lookup"><span data-stu-id="beba6-196">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="beba6-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="beba6-197">Response</span></span>

<span data-ttu-id="beba6-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="beba6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="beba6-201">Endpunktprüfung für Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="beba6-201">Notification endpoint validation</span></span>

<span data-ttu-id="beba6-202">Der Abonnement Benachrichtigungs Endpunkt (in der `notificationUrl` Eigenschaft angegeben) muss auf eine Validierungs Anforderung reagieren können, wie unter [Einrichten von Benachrichtigungen für Änderungen in Benutzerdaten](/graph/webhooks#notification-endpoint-validation)beschrieben.</span><span class="sxs-lookup"><span data-stu-id="beba6-202">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="beba6-203">Wenn die Validierung fehlschlägt, gibt die Anforderung zum Erstellen des Abonnements einen Fehler vom 400 unGültigen Anforderung zurück.</span><span class="sxs-lookup"><span data-stu-id="beba6-203">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
