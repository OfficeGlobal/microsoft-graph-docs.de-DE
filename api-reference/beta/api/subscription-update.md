---
title: Abonnement aktualisieren
description: Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 19355ff8acbcdade689b140abca63e8d9885e3fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512780"
---
# <a name="update-subscription"></a><span data-ttu-id="a72fa-103">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a72fa-103">Update subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a72fa-104">Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="a72fa-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="a72fa-105">Abonnements laufen ab nach der Zeitspanne, die nach Ressourcentyp variiert.</span><span class="sxs-lookup"><span data-stu-id="a72fa-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="a72fa-106">Zur Vermeidung von Benachrichtigungen fehlende sollten eine app seine Abonnements im Vorfeld ihrem Ablaufdatum erneuern.</span><span class="sxs-lookup"><span data-stu-id="a72fa-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="a72fa-107">Finden Sie unter [Abonnement](../resources/subscription.md) für die maximale Länge eines Abonnements für jeden Ressourcentyp.</span><span class="sxs-lookup"><span data-stu-id="a72fa-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="a72fa-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a72fa-108">Permissions</span></span>

<span data-ttu-id="a72fa-p102">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a72fa-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a72fa-111">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="a72fa-111">Resource type / Item</span></span>        | <span data-ttu-id="a72fa-112">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="a72fa-112">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="a72fa-113">Kontakte</span><span class="sxs-lookup"><span data-stu-id="a72fa-113">Contacts</span></span>                    | <span data-ttu-id="a72fa-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a72fa-114">Contacts.Read</span></span>       |
| <span data-ttu-id="a72fa-115">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="a72fa-115">Conversations</span></span>               | <span data-ttu-id="a72fa-116">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a72fa-116">Group.Read.All</span></span>      |
| <span data-ttu-id="a72fa-117">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="a72fa-117">Events</span></span>                      | <span data-ttu-id="a72fa-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a72fa-118">Calendars.Read</span></span>      |
| <span data-ttu-id="a72fa-119">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="a72fa-119">Messages</span></span>                    | <span data-ttu-id="a72fa-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a72fa-120">Mail.Read</span></span>           |
| <span data-ttu-id="a72fa-121">Gruppen</span><span class="sxs-lookup"><span data-stu-id="a72fa-121">Groups</span></span>                      | <span data-ttu-id="a72fa-122">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a72fa-122">Group.Read.All</span></span>      |
| <span data-ttu-id="a72fa-123">Benutzer</span><span class="sxs-lookup"><span data-stu-id="a72fa-123">Users</span></span>                       | <span data-ttu-id="a72fa-124">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a72fa-124">User.Read.All</span></span>       |
| <span data-ttu-id="a72fa-125">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="a72fa-125">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="a72fa-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a72fa-126">Files.ReadWrite</span></span>     |
| <span data-ttu-id="a72fa-127">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="a72fa-127">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="a72fa-128">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a72fa-128">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="a72fa-129">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="a72fa-129">Security alert</span></span>               | <span data-ttu-id="a72fa-130">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a72fa-130">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="a72fa-131">***Hinweis:*** Der Endpunkt /beta kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="a72fa-131">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="a72fa-132">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a72fa-132">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="a72fa-133">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a72fa-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a72fa-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a72fa-134">Request headers</span></span>

| <span data-ttu-id="a72fa-135">Name</span><span class="sxs-lookup"><span data-stu-id="a72fa-135">Name</span></span>       | <span data-ttu-id="a72fa-136">Typ</span><span class="sxs-lookup"><span data-stu-id="a72fa-136">Type</span></span> | <span data-ttu-id="a72fa-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a72fa-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a72fa-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="a72fa-138">Authorization</span></span>  | <span data-ttu-id="a72fa-139">string</span><span class="sxs-lookup"><span data-stu-id="a72fa-139">string</span></span>  | <span data-ttu-id="a72fa-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a72fa-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a72fa-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="a72fa-142">Response</span></span>

<span data-ttu-id="a72fa-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a72fa-143">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a72fa-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a72fa-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a72fa-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a72fa-145">Request</span></span>

<span data-ttu-id="a72fa-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a72fa-146">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a72fa-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="a72fa-147">Response</span></span>

<span data-ttu-id="a72fa-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a72fa-148">Here is an example of the response.</span></span>
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

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
