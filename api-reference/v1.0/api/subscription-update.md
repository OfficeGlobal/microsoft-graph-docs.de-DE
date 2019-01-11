---
title: Abonnement aktualisieren
description: Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.
localization_priority: Normal
ms.openlocfilehash: f0804421c2e178d176975317ba82bb0aac0ae212
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809716"
---
# <a name="update-subscription"></a><span data-ttu-id="6a80f-103">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6a80f-103">Update subscription</span></span>

<span data-ttu-id="6a80f-104">Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="6a80f-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="6a80f-105">Abonnements laufen ab nach der Zeitspanne, die nach Ressourcentyp variiert.</span><span class="sxs-lookup"><span data-stu-id="6a80f-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="6a80f-106">Zur Vermeidung von Benachrichtigungen fehlende sollten eine app seine Abonnements im Vorfeld ihrem Ablaufdatum erneuern.</span><span class="sxs-lookup"><span data-stu-id="6a80f-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="6a80f-107">Finden Sie unter [Abonnement](../resources/subscription.md) für die maximale Länge eines Abonnements für jeden Ressourcentyp.</span><span class="sxs-lookup"><span data-stu-id="6a80f-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a80f-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6a80f-108">Permissions</span></span>

<span data-ttu-id="6a80f-p102">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a80f-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a80f-111">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="6a80f-111">Resource type / Item</span></span>        | <span data-ttu-id="6a80f-112">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="6a80f-112">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="6a80f-113">Kontakte</span><span class="sxs-lookup"><span data-stu-id="6a80f-113">Contacts</span></span>                    | <span data-ttu-id="6a80f-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6a80f-114">Contacts.Read</span></span>       |
| <span data-ttu-id="6a80f-115">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="6a80f-115">Conversations</span></span>               | <span data-ttu-id="6a80f-116">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a80f-116">Group.Read.All</span></span>      |
| <span data-ttu-id="6a80f-117">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="6a80f-117">Events</span></span>                      | <span data-ttu-id="6a80f-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6a80f-118">Calendars.Read</span></span>      |
| <span data-ttu-id="6a80f-119">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="6a80f-119">Messages</span></span>                    | <span data-ttu-id="6a80f-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6a80f-120">Mail.Read</span></span>           |
| <span data-ttu-id="6a80f-121">Gruppen</span><span class="sxs-lookup"><span data-stu-id="6a80f-121">Groups</span></span>                      | <span data-ttu-id="6a80f-122">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a80f-122">Group.Read.All</span></span>      |
| <span data-ttu-id="6a80f-123">Benutzer</span><span class="sxs-lookup"><span data-stu-id="6a80f-123">Users</span></span>                       | <span data-ttu-id="6a80f-124">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a80f-124">User.Read.All</span></span>       |
| <span data-ttu-id="6a80f-125">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="6a80f-125">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="6a80f-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a80f-126">Files.ReadWrite</span></span>     |
| <span data-ttu-id="6a80f-127">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="6a80f-127">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="6a80f-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a80f-128">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="6a80f-129">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="6a80f-129">Security alert</span></span>| <span data-ttu-id="6a80f-130">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a80f-130">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a80f-131">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a80f-131">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6a80f-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a80f-132">Request headers</span></span>

| <span data-ttu-id="6a80f-133">Name</span><span class="sxs-lookup"><span data-stu-id="6a80f-133">Name</span></span>       | <span data-ttu-id="6a80f-134">Typ</span><span class="sxs-lookup"><span data-stu-id="6a80f-134">Type</span></span> | <span data-ttu-id="6a80f-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a80f-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a80f-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a80f-136">Authorization</span></span>  | <span data-ttu-id="6a80f-137">string</span><span class="sxs-lookup"><span data-stu-id="6a80f-137">string</span></span>  | <span data-ttu-id="6a80f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a80f-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6a80f-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a80f-140">Response</span></span>

<span data-ttu-id="6a80f-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a80f-141">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a80f-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a80f-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6a80f-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a80f-143">Request</span></span>

<span data-ttu-id="6a80f-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a80f-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a><span data-ttu-id="6a80f-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a80f-145">Response</span></span>

<span data-ttu-id="6a80f-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6a80f-146">Here is an example of the response.</span></span>
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
  "clientState":"subscription-identifier",
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
