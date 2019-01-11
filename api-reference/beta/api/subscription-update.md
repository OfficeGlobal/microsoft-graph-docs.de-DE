---
title: Abonnement aktualisieren
description: Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.
localization_priority: Normal
ms.openlocfilehash: 63bcf8f4084053356819601cd6306ad3ff5238c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836120"
---
# <a name="update-subscription"></a><span data-ttu-id="a04e9-103">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a04e9-103">Update subscription</span></span>

> <span data-ttu-id="a04e9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a04e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a04e9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a04e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a04e9-106">Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="a04e9-106">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="a04e9-107">Abonnements laufen ab nach der Zeitspanne, die nach Ressourcentyp variiert.</span><span class="sxs-lookup"><span data-stu-id="a04e9-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="a04e9-108">Zur Vermeidung von Benachrichtigungen fehlende sollten eine app seine Abonnements im Vorfeld ihrem Ablaufdatum erneuern.</span><span class="sxs-lookup"><span data-stu-id="a04e9-108">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="a04e9-109">Finden Sie unter [Abonnement](../resources/subscription.md) für die maximale Länge eines Abonnements für jeden Ressourcentyp.</span><span class="sxs-lookup"><span data-stu-id="a04e9-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="a04e9-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a04e9-110">Permissions</span></span>

<span data-ttu-id="a04e9-p103">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a04e9-p103">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a04e9-113">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="a04e9-113">Resource type / Item</span></span>        | <span data-ttu-id="a04e9-114">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="a04e9-114">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="a04e9-115">Kontakte</span><span class="sxs-lookup"><span data-stu-id="a04e9-115">Contacts</span></span>                    | <span data-ttu-id="a04e9-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a04e9-116">Contacts.Read</span></span>       |
| <span data-ttu-id="a04e9-117">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="a04e9-117">Conversations</span></span>               | <span data-ttu-id="a04e9-118">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a04e9-118">Group.Read.All</span></span>      |
| <span data-ttu-id="a04e9-119">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="a04e9-119">Events</span></span>                      | <span data-ttu-id="a04e9-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a04e9-120">Calendars.Read</span></span>      |
| <span data-ttu-id="a04e9-121">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="a04e9-121">Messages</span></span>                    | <span data-ttu-id="a04e9-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a04e9-122">Mail.Read</span></span>           |
| <span data-ttu-id="a04e9-123">Gruppen</span><span class="sxs-lookup"><span data-stu-id="a04e9-123">Groups</span></span>                      | <span data-ttu-id="a04e9-124">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a04e9-124">Group.Read.All</span></span>      |
| <span data-ttu-id="a04e9-125">Benutzer</span><span class="sxs-lookup"><span data-stu-id="a04e9-125">Users</span></span>                       | <span data-ttu-id="a04e9-126">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a04e9-126">User.Read.All</span></span>       |
| <span data-ttu-id="a04e9-127">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="a04e9-127">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="a04e9-128">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a04e9-128">Files.ReadWrite</span></span>     |
| <span data-ttu-id="a04e9-129">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="a04e9-129">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="a04e9-130">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a04e9-130">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="a04e9-131">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="a04e9-131">Security alert</span></span>               | <span data-ttu-id="a04e9-132">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a04e9-132">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="a04e9-133">***Hinweis:*** Der Endpunkt /beta kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="a04e9-133">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="a04e9-134">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a04e9-134">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="a04e9-135">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a04e9-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a04e9-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a04e9-136">Request headers</span></span>

| <span data-ttu-id="a04e9-137">Name</span><span class="sxs-lookup"><span data-stu-id="a04e9-137">Name</span></span>       | <span data-ttu-id="a04e9-138">Typ</span><span class="sxs-lookup"><span data-stu-id="a04e9-138">Type</span></span> | <span data-ttu-id="a04e9-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a04e9-139">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a04e9-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="a04e9-140">Authorization</span></span>  | <span data-ttu-id="a04e9-141">string</span><span class="sxs-lookup"><span data-stu-id="a04e9-141">string</span></span>  | <span data-ttu-id="a04e9-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a04e9-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a04e9-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="a04e9-144">Response</span></span>

<span data-ttu-id="a04e9-145">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a04e9-145">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a04e9-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a04e9-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a04e9-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a04e9-147">Request</span></span>

<span data-ttu-id="a04e9-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a04e9-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="a04e9-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="a04e9-149">Response</span></span>

<span data-ttu-id="a04e9-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a04e9-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
