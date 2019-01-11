---
title: Abonnement erstellen
description: Abonniert Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Daten in einem Microsoft Graph-Ressource geändert.
localization_priority: Normal
ms.openlocfilehash: 5b7f465e556d1fb752bcb2d3c962fd6444d462c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805054"
---
# <a name="create-subscription"></a><span data-ttu-id="0ee1b-103">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="0ee1b-103">Create subscription</span></span>

> <span data-ttu-id="0ee1b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ee1b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ee1b-106">Abonniert Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Daten in einem Microsoft Graph-Ressource geändert.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-106">Subscribes a listener application to receive notifications when data on a Microsoft Graph resource changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ee1b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0ee1b-107">Permissions</span></span>

<span data-ttu-id="0ee1b-108">Erstellen eines Abonnements erfordert Leseberechtigung für die Ressource für die die app Benachrichtigungen empfangen wird.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-108">Creating a subscription requires read permission to the resource for which the app will receive notifications.</span></span> <span data-ttu-id="0ee1b-109">Wenn Benachrichtigungen zu Nachrichten erhalten möchten, beispielsweise Ihre app muss die `Mail.Read` Berechtigung.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-109">For example, to get notifications about Messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="0ee1b-110">Die folgende Tabelle listet die vorgeschlagenen Berechtigungen, die für die jeweilige Ressource erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-110">The following table lists the suggested permission needed for each resource.</span></span> <span data-ttu-id="0ee1b-111">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee1b-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ee1b-112">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="0ee1b-112">Resource type / Item</span></span>        | <span data-ttu-id="0ee1b-113">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="0ee1b-113">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="0ee1b-114">Kontakte</span><span class="sxs-lookup"><span data-stu-id="0ee1b-114">Contacts</span></span>                    | <span data-ttu-id="0ee1b-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0ee1b-115">Contacts.Read</span></span>       |
| <span data-ttu-id="0ee1b-116">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="0ee1b-116">Conversations</span></span>               | <span data-ttu-id="0ee1b-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ee1b-117">Group.Read.All</span></span>      |
| <span data-ttu-id="0ee1b-118">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="0ee1b-118">Events</span></span>                      | <span data-ttu-id="0ee1b-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="0ee1b-119">Calendars.Read</span></span>      |
| <span data-ttu-id="0ee1b-120">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="0ee1b-120">Messages</span></span>                    | <span data-ttu-id="0ee1b-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="0ee1b-121">Mail.Read</span></span>           |
| <span data-ttu-id="0ee1b-122">Gruppen</span><span class="sxs-lookup"><span data-stu-id="0ee1b-122">Groups</span></span>                      | <span data-ttu-id="0ee1b-123">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ee1b-123">Group.Read.All</span></span>      |
| <span data-ttu-id="0ee1b-124">Benutzer</span><span class="sxs-lookup"><span data-stu-id="0ee1b-124">Users</span></span>                       | <span data-ttu-id="0ee1b-125">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ee1b-125">User.Read.All</span></span>       |
| <span data-ttu-id="0ee1b-126">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="0ee1b-126">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="0ee1b-127">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ee1b-127">Files.ReadWrite</span></span>     |
| <span data-ttu-id="0ee1b-128">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="0ee1b-128">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="0ee1b-129">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee1b-129">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="0ee1b-130">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="0ee1b-130">Security alert</span></span>              | <span data-ttu-id="0ee1b-131">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee1b-131">SecurityEvents.ReadWrite.All</span></span> |

> <span data-ttu-id="0ee1b-132">**Hinweis:** Der Endpunkt /beta kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-132">**Note:** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="0ee1b-133">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-133">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="0ee1b-134">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ee1b-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="0ee1b-135">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ee1b-135">Request headers</span></span>

| <span data-ttu-id="0ee1b-136">Name</span><span class="sxs-lookup"><span data-stu-id="0ee1b-136">Name</span></span>       | <span data-ttu-id="0ee1b-137">Typ</span><span class="sxs-lookup"><span data-stu-id="0ee1b-137">Type</span></span> | <span data-ttu-id="0ee1b-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ee1b-138">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0ee1b-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ee1b-139">Authorization</span></span>  | <span data-ttu-id="0ee1b-140">string</span><span class="sxs-lookup"><span data-stu-id="0ee1b-140">string</span></span>  | <span data-ttu-id="0ee1b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0ee1b-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ee1b-143">Response</span></span>

<span data-ttu-id="0ee1b-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-144">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ee1b-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ee1b-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0ee1b-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ee1b-146">Request</span></span>

<span data-ttu-id="0ee1b-147">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Abonnement](../resources/subscription.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-147">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="0ee1b-148">Die `clientState` Feld ist optional.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-148">The `clientState` field is optional.</span></span>

<span data-ttu-id="0ee1b-149">In diesem Beispiel für eine Anforderung erstellt ein Abonnement für Benachrichtigungen zu neuen e-Mail-Nachrichten von den derzeit angemeldeten Benutzer empfangen.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-149">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
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

<span data-ttu-id="0ee1b-150">Folgende sind gültige Werte für die Ressourceneigenschaft:</span><span class="sxs-lookup"><span data-stu-id="0ee1b-150">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="0ee1b-151">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0ee1b-151">Resource type</span></span> | <span data-ttu-id="0ee1b-152">Beispiele</span><span class="sxs-lookup"><span data-stu-id="0ee1b-152">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="0ee1b-153">Mail</span><span class="sxs-lookup"><span data-stu-id="0ee1b-153">Mail</span></span>|<span data-ttu-id="0ee1b-154">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="0ee1b-154">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="0ee1b-155">me/messages</span><span class="sxs-lookup"><span data-stu-id="0ee1b-155">me/messages</span></span>|
|<span data-ttu-id="0ee1b-156">Kontakte</span><span class="sxs-lookup"><span data-stu-id="0ee1b-156">Contacts</span></span>|<span data-ttu-id="0ee1b-157">me/contacts</span><span class="sxs-lookup"><span data-stu-id="0ee1b-157">me/contacts</span></span>|
|<span data-ttu-id="0ee1b-158">Kalender</span><span class="sxs-lookup"><span data-stu-id="0ee1b-158">Calendars</span></span>|<span data-ttu-id="0ee1b-159">me/events</span><span class="sxs-lookup"><span data-stu-id="0ee1b-159">me/events</span></span>|
|<span data-ttu-id="0ee1b-160">Benutzer</span><span class="sxs-lookup"><span data-stu-id="0ee1b-160">Users</span></span>|<span data-ttu-id="0ee1b-161">users</span><span class="sxs-lookup"><span data-stu-id="0ee1b-161">users</span></span>|
|<span data-ttu-id="0ee1b-162">Gruppen</span><span class="sxs-lookup"><span data-stu-id="0ee1b-162">Groups</span></span>|<span data-ttu-id="0ee1b-163">Gruppen</span><span class="sxs-lookup"><span data-stu-id="0ee1b-163">groups</span></span>|
|<span data-ttu-id="0ee1b-164">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="0ee1b-164">Conversations</span></span>|<span data-ttu-id="0ee1b-165">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="0ee1b-165">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="0ee1b-166">Laufwerke</span><span class="sxs-lookup"><span data-stu-id="0ee1b-166">Drives</span></span>|<span data-ttu-id="0ee1b-167">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="0ee1b-167">me/drive/root</span></span>|
|<span data-ttu-id="0ee1b-168">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="0ee1b-168">Security alert</span></span>|<span data-ttu-id="0ee1b-169">Sicherheitshinweise /? $filter = Status Eq 'Neu'</span><span class="sxs-lookup"><span data-stu-id="0ee1b-169">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="0ee1b-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ee1b-170">Response</span></span>

<span data-ttu-id="0ee1b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="0ee1b-174">Endpunktprüfung für Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="0ee1b-174">Notification endpoint validation</span></span>

<span data-ttu-id="0ee1b-175">Das Abonnement Benachrichtigung Endpunkt (im angegebenen der `notificationUrl` -Eigenschaft) müssen Daten aneinander zur Reaktion auf eine Anforderung zur Überprüfung, wie unter [Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="0ee1b-175">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="0ee1b-176">Wenn die Überprüfung fehlschlägt, gibt die Anforderung an das Abonnement zu erstellen einer 400-Bad Request-Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="0ee1b-176">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
