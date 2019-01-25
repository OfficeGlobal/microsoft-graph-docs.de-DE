---
title: Abonnement erstellen
description: Abonniert Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Daten in einem Microsoft Graph-Ressource geändert.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 002dd88c7db2650be2303e7df6f86ce9a5fbdaa9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527577"
---
# <a name="create-subscription"></a><span data-ttu-id="67428-103">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="67428-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67428-104">Abonniert Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Daten in einem Microsoft Graph-Ressource geändert.</span><span class="sxs-lookup"><span data-stu-id="67428-104">Subscribes a listener application to receive notifications when data on a Microsoft Graph resource changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="67428-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="67428-105">Permissions</span></span>

<span data-ttu-id="67428-106">Erstellen eines Abonnements erfordert Leseberechtigung für die Ressource für die die app Benachrichtigungen empfangen wird.</span><span class="sxs-lookup"><span data-stu-id="67428-106">Creating a subscription requires read permission to the resource for which the app will receive notifications.</span></span> <span data-ttu-id="67428-107">Wenn Benachrichtigungen zu Nachrichten erhalten möchten, beispielsweise Ihre app muss die `Mail.Read` Berechtigung.</span><span class="sxs-lookup"><span data-stu-id="67428-107">For example, to get notifications about Messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="67428-108">Die folgende Tabelle listet die vorgeschlagenen Berechtigungen, die für die jeweilige Ressource erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="67428-108">The following table lists the suggested permission needed for each resource.</span></span> <span data-ttu-id="67428-109">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67428-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67428-110">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="67428-110">Resource type / Item</span></span>        | <span data-ttu-id="67428-111">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="67428-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="67428-112">Kontakte</span><span class="sxs-lookup"><span data-stu-id="67428-112">Contacts</span></span>                    | <span data-ttu-id="67428-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="67428-113">Contacts.Read</span></span>       |
| <span data-ttu-id="67428-114">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="67428-114">Conversations</span></span>               | <span data-ttu-id="67428-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="67428-115">Group.Read.All</span></span>      |
| <span data-ttu-id="67428-116">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="67428-116">Events</span></span>                      | <span data-ttu-id="67428-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="67428-117">Calendars.Read</span></span>      |
| <span data-ttu-id="67428-118">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="67428-118">Messages</span></span>                    | <span data-ttu-id="67428-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="67428-119">Mail.Read</span></span>           |
| <span data-ttu-id="67428-120">Gruppen</span><span class="sxs-lookup"><span data-stu-id="67428-120">Groups</span></span>                      | <span data-ttu-id="67428-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="67428-121">Group.Read.All</span></span>      |
| <span data-ttu-id="67428-122">Benutzer</span><span class="sxs-lookup"><span data-stu-id="67428-122">Users</span></span>                       | <span data-ttu-id="67428-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="67428-123">User.Read.All</span></span>       |
| <span data-ttu-id="67428-124">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="67428-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="67428-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67428-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="67428-126">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="67428-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="67428-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67428-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="67428-128">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="67428-128">Security alert</span></span>              | <span data-ttu-id="67428-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67428-129">SecurityEvents.ReadWrite.All</span></span> |

> <span data-ttu-id="67428-130">**Hinweis:** Der Endpunkt /beta kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="67428-130">**Note:** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="67428-131">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67428-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="67428-132">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="67428-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="67428-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="67428-133">Request headers</span></span>

| <span data-ttu-id="67428-134">Name</span><span class="sxs-lookup"><span data-stu-id="67428-134">Name</span></span>       | <span data-ttu-id="67428-135">Typ</span><span class="sxs-lookup"><span data-stu-id="67428-135">Type</span></span> | <span data-ttu-id="67428-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67428-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="67428-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="67428-137">Authorization</span></span>  | <span data-ttu-id="67428-138">string</span><span class="sxs-lookup"><span data-stu-id="67428-138">string</span></span>  | <span data-ttu-id="67428-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="67428-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="67428-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="67428-141">Response</span></span>

<span data-ttu-id="67428-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67428-142">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67428-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="67428-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="67428-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="67428-144">Request</span></span>

<span data-ttu-id="67428-145">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Abonnement](../resources/subscription.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="67428-145">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="67428-146">Die `clientState` Feld ist optional.</span><span class="sxs-lookup"><span data-stu-id="67428-146">The `clientState` field is optional.</span></span>

<span data-ttu-id="67428-147">In diesem Beispiel für eine Anforderung erstellt ein Abonnement für Benachrichtigungen zu neuen e-Mail-Nachrichten von den derzeit angemeldeten Benutzer empfangen.</span><span class="sxs-lookup"><span data-stu-id="67428-147">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
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

<span data-ttu-id="67428-148">Folgende sind gültige Werte für die Ressourceneigenschaft:</span><span class="sxs-lookup"><span data-stu-id="67428-148">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="67428-149">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="67428-149">Resource type</span></span> | <span data-ttu-id="67428-150">Beispiele</span><span class="sxs-lookup"><span data-stu-id="67428-150">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="67428-151">Mail</span><span class="sxs-lookup"><span data-stu-id="67428-151">Mail</span></span>|<span data-ttu-id="67428-152">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="67428-152">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="67428-153">me/messages</span><span class="sxs-lookup"><span data-stu-id="67428-153">me/messages</span></span>|
|<span data-ttu-id="67428-154">Kontakte</span><span class="sxs-lookup"><span data-stu-id="67428-154">Contacts</span></span>|<span data-ttu-id="67428-155">me/contacts</span><span class="sxs-lookup"><span data-stu-id="67428-155">me/contacts</span></span>|
|<span data-ttu-id="67428-156">Kalender</span><span class="sxs-lookup"><span data-stu-id="67428-156">Calendars</span></span>|<span data-ttu-id="67428-157">me/events</span><span class="sxs-lookup"><span data-stu-id="67428-157">me/events</span></span>|
|<span data-ttu-id="67428-158">Benutzer</span><span class="sxs-lookup"><span data-stu-id="67428-158">Users</span></span>|<span data-ttu-id="67428-159">users</span><span class="sxs-lookup"><span data-stu-id="67428-159">users</span></span>|
|<span data-ttu-id="67428-160">Gruppen</span><span class="sxs-lookup"><span data-stu-id="67428-160">Groups</span></span>|<span data-ttu-id="67428-161">Gruppen</span><span class="sxs-lookup"><span data-stu-id="67428-161">groups</span></span>|
|<span data-ttu-id="67428-162">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="67428-162">Conversations</span></span>|<span data-ttu-id="67428-163">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="67428-163">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="67428-164">Laufwerke</span><span class="sxs-lookup"><span data-stu-id="67428-164">Drives</span></span>|<span data-ttu-id="67428-165">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="67428-165">me/drive/root</span></span>|
|<span data-ttu-id="67428-166">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="67428-166">Security alert</span></span>|<span data-ttu-id="67428-167">Sicherheitshinweise /? $filter = Status Eq 'Neu'</span><span class="sxs-lookup"><span data-stu-id="67428-167">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="67428-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="67428-168">Response</span></span>

<span data-ttu-id="67428-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="67428-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="67428-172">Endpunktprüfung für Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="67428-172">Notification endpoint validation</span></span>

<span data-ttu-id="67428-173">Das Abonnement Benachrichtigung Endpunkt (im angegebenen der `notificationUrl` -Eigenschaft) müssen Daten aneinander zur Reaktion auf eine Anforderung zur Überprüfung, wie unter [Einrichten von Benachrichtigungen, damit die Änderungen in Benutzerdaten](/graph/webhooks#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="67428-173">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="67428-174">Wenn die Überprüfung fehlschlägt, gibt die Anforderung an das Abonnement zu erstellen einer 400-Bad Request-Fehler zurück.</span><span class="sxs-lookup"><span data-stu-id="67428-174">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
