---
title: Abonnement erstellen
description: Diese API abonniert eine Listeneranwendung, über die sie Benachrichtigungen erhält, sobald Daten in Microsoft Graph geändert werden
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 7b23968620abcb8f9a20e4a7b3598c21dec72980
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913886"
---
# <a name="create-subscription"></a><span data-ttu-id="299f0-103">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="299f0-103">Create subscription</span></span>

<span data-ttu-id="299f0-104">Diese API abonniert eine Listeneranwendung, über die sie Benachrichtigungen erhält, sobald Daten in Microsoft Graph geändert werden</span><span class="sxs-lookup"><span data-stu-id="299f0-104">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="299f0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="299f0-105">Permissions</span></span>

<span data-ttu-id="299f0-p101">Zur Abonnementerstellung ist Lesezugriff auf die Ressource erforderlich. Beispiel: um Benachrichtigungsnachrichten zu erhalten, benötigt Ihre App die `Mail.Read`-Berechtigung. In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="299f0-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="299f0-110">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="299f0-110">Resource type / Item</span></span>        | <span data-ttu-id="299f0-111">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="299f0-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="299f0-112">Kontakte</span><span class="sxs-lookup"><span data-stu-id="299f0-112">Contacts</span></span>                    | <span data-ttu-id="299f0-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="299f0-113">Contacts.Read</span></span>       |
| <span data-ttu-id="299f0-114">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="299f0-114">Conversations</span></span>               | <span data-ttu-id="299f0-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="299f0-115">Group.Read.All</span></span>      |
| <span data-ttu-id="299f0-116">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="299f0-116">Events</span></span>                      | <span data-ttu-id="299f0-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="299f0-117">Calendars.Read</span></span>      |
| <span data-ttu-id="299f0-118">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="299f0-118">Messages</span></span>                    | <span data-ttu-id="299f0-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="299f0-119">Mail.Read</span></span>           |
| <span data-ttu-id="299f0-120">Gruppen</span><span class="sxs-lookup"><span data-stu-id="299f0-120">Groups</span></span>                      | <span data-ttu-id="299f0-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="299f0-121">Group.Read.All</span></span>      |
| <span data-ttu-id="299f0-122">Benutzer</span><span class="sxs-lookup"><span data-stu-id="299f0-122">Users</span></span>                       | <span data-ttu-id="299f0-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="299f0-123">User.Read.All</span></span>       |
| <span data-ttu-id="299f0-124">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="299f0-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="299f0-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="299f0-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="299f0-126">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="299f0-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="299f0-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="299f0-127">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="299f0-128">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="299f0-128">Security alert</span></span>| <span data-ttu-id="299f0-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="299f0-129">SecurityEvents.ReadWrite.All</span></span> |

 > <span data-ttu-id="299f0-130">**Hinweis:** Der Endpunkt /v1.0 kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="299f0-130">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="299f0-131">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="299f0-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="299f0-132">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="299f0-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="299f0-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="299f0-133">Request headers</span></span>

| <span data-ttu-id="299f0-134">Name</span><span class="sxs-lookup"><span data-stu-id="299f0-134">Name</span></span>       | <span data-ttu-id="299f0-135">Typ</span><span class="sxs-lookup"><span data-stu-id="299f0-135">Type</span></span> | <span data-ttu-id="299f0-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="299f0-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="299f0-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="299f0-137">Authorization</span></span>  | <span data-ttu-id="299f0-138">string</span><span class="sxs-lookup"><span data-stu-id="299f0-138">string</span></span>  | <span data-ttu-id="299f0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="299f0-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="299f0-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="299f0-141">Response</span></span>

<span data-ttu-id="299f0-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="299f0-142">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="299f0-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="299f0-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="299f0-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="299f0-144">Request</span></span>

<span data-ttu-id="299f0-145">Hier sehen Sie ein Beispiel für die Anforderung zum Senden einer Benachrichtigung, wenn der Benutzer eine neue E-Mail empfängt.</span><span class="sxs-lookup"><span data-stu-id="299f0-145">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
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

<span data-ttu-id="299f0-146">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Abonnement](../resources/subscription.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="299f0-146">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="299f0-147">Die `clientState` Feld ist optional.</span><span class="sxs-lookup"><span data-stu-id="299f0-147">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="299f0-148">Beispiele für Ressourcen</span><span class="sxs-lookup"><span data-stu-id="299f0-148">Resources examples</span></span>

<span data-ttu-id="299f0-149">Im Folgenden sind gültige Werte für die Ressourceneigenschaft des Abonnements aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="299f0-149">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="299f0-150">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="299f0-150">Resource type</span></span> | <span data-ttu-id="299f0-151">Beispiele</span><span class="sxs-lookup"><span data-stu-id="299f0-151">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="299f0-152">Mail</span><span class="sxs-lookup"><span data-stu-id="299f0-152">Mail</span></span>|<span data-ttu-id="299f0-153">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="299f0-153">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="299f0-154">me/messages</span><span class="sxs-lookup"><span data-stu-id="299f0-154">me/messages</span></span>|
|<span data-ttu-id="299f0-155">Kontakte</span><span class="sxs-lookup"><span data-stu-id="299f0-155">Contacts</span></span>|<span data-ttu-id="299f0-156">me/contacts</span><span class="sxs-lookup"><span data-stu-id="299f0-156">me/contacts</span></span>|
|<span data-ttu-id="299f0-157">Kalender</span><span class="sxs-lookup"><span data-stu-id="299f0-157">Calendars</span></span>|<span data-ttu-id="299f0-158">me/events</span><span class="sxs-lookup"><span data-stu-id="299f0-158">me/events</span></span>|
|<span data-ttu-id="299f0-159">Benutzer</span><span class="sxs-lookup"><span data-stu-id="299f0-159">Users</span></span>|<span data-ttu-id="299f0-160">users</span><span class="sxs-lookup"><span data-stu-id="299f0-160">users</span></span>|
|<span data-ttu-id="299f0-161">Gruppen</span><span class="sxs-lookup"><span data-stu-id="299f0-161">Groups</span></span>|<span data-ttu-id="299f0-162">Gruppen</span><span class="sxs-lookup"><span data-stu-id="299f0-162">groups</span></span>|
|<span data-ttu-id="299f0-163">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="299f0-163">Conversations</span></span>|<span data-ttu-id="299f0-164">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="299f0-164">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="299f0-165">Laufwerke</span><span class="sxs-lookup"><span data-stu-id="299f0-165">Drives</span></span>|<span data-ttu-id="299f0-166">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="299f0-166">me/drive/root</span></span>|
|<span data-ttu-id="299f0-167">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="299f0-167">Security alert</span></span>|<span data-ttu-id="299f0-168">Sicherheitshinweise /? $filter = Status Eq 'Neu'</span><span class="sxs-lookup"><span data-stu-id="299f0-168">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="299f0-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="299f0-169">Response</span></span>

<span data-ttu-id="299f0-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="299f0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="299f0-173">Endpunktprüfung für Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="299f0-173">Notification endpoint validation</span></span>

<span data-ttu-id="299f0-174">Das Abonnement Benachrichtigung Endpunkt (im angegebenen der `notificationUrl` -Eigenschaft) müssen Daten aneinander zur Reaktion auf eine Anforderung zur Überprüfung, wie unter [Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="299f0-174">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="299f0-175">Wenn die Überprüfung fehlschlägt, gibt die Anforderung an das Abonnement zu erstellen einer 400-Bad Request-Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="299f0-175">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
