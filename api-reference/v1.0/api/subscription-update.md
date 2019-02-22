---
title: Abonnement aktualisieren
description: Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 1bf693fb8551db916807570459d9658fa02665f1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167802"
---
# <a name="update-subscription"></a><span data-ttu-id="16131-103">Abonnement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="16131-103">Update subscription</span></span>

<span data-ttu-id="16131-104">Erneuert ein Abonnement durch Verlängern seiner Ablaufzeit.</span><span class="sxs-lookup"><span data-stu-id="16131-104">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="16131-105">Abonnements laufen nach einer vom Ressourcentyp unterschiedlichen Zeitspanne ab.</span><span class="sxs-lookup"><span data-stu-id="16131-105">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="16131-106">Um fehlende Benachrichtigungen zu vermeiden, sollte eine APP Ihre Abonnements vor Ablauf des Gültigkeitszeitraums verlängern.</span><span class="sxs-lookup"><span data-stu-id="16131-106">In order to avoid missing notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="16131-107">Weitere Informationen finden Sie unter [Abonnement](../resources/subscription.md) für die maximale Länge eines Abonnements für die einzelnen Ressourcentypen.</span><span class="sxs-lookup"><span data-stu-id="16131-107">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="16131-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="16131-108">Permissions</span></span>

<span data-ttu-id="16131-109">Abhängig von der angeforderten Ressource und dem Berechtigungstyp (Delegierte oder Anwendung) ist die in der folgenden Tabelle angegebene Berechtigung die am wenigsten privilegierten Berechtigungen zum Aufrufen dieser API.</span><span class="sxs-lookup"><span data-stu-id="16131-109">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="16131-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16131-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16131-111">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="16131-111">Supported resource</span></span> | <span data-ttu-id="16131-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="16131-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16131-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="16131-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16131-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="16131-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="16131-115">Kontakt</span><span class="sxs-lookup"><span data-stu-id="16131-115">contact</span></span>](../resources/contact.md) | <span data-ttu-id="16131-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="16131-116">Contacts.Read</span></span> | <span data-ttu-id="16131-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="16131-117">Contacts.Read</span></span> | <span data-ttu-id="16131-118">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="16131-118">Contacts.Read</span></span> |
|<span data-ttu-id="16131-119">[driveItem](../resources/driveitem.md) (persönliche OneDrive des Benutzers)</span><span class="sxs-lookup"><span data-stu-id="16131-119">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="16131-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16131-120">Not supported</span></span> | <span data-ttu-id="16131-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16131-121">Files.ReadWrite</span></span> | <span data-ttu-id="16131-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16131-122">Not supported</span></span> |
|<span data-ttu-id="16131-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="16131-123">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="16131-124">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16131-124">Files.ReadWrite.All</span></span> | <span data-ttu-id="16131-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16131-125">Not supported</span></span> | <span data-ttu-id="16131-126">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16131-126">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="16131-127">event</span><span class="sxs-lookup"><span data-stu-id="16131-127">event</span></span>](../resources/event.md) | <span data-ttu-id="16131-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="16131-128">Calendars.Read</span></span> | <span data-ttu-id="16131-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="16131-129">Calendars.Read</span></span> | <span data-ttu-id="16131-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="16131-130">Calendars.Read</span></span> |
|[<span data-ttu-id="16131-131">group</span><span class="sxs-lookup"><span data-stu-id="16131-131">group</span></span>](../resources/group.md) | <span data-ttu-id="16131-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="16131-132">Group.Read.All</span></span> | <span data-ttu-id="16131-133">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16131-133">Not supported</span></span> | <span data-ttu-id="16131-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="16131-134">Group.Read.All</span></span> |
|[<span data-ttu-id="16131-135">Gruppenunterhaltung</span><span class="sxs-lookup"><span data-stu-id="16131-135">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="16131-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="16131-136">Group.Read.All</span></span> | <span data-ttu-id="16131-137">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16131-137">Not supported</span></span> | <span data-ttu-id="16131-138">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16131-138">Not supported</span></span> |
|[<span data-ttu-id="16131-139">Nachricht</span><span class="sxs-lookup"><span data-stu-id="16131-139">message</span></span>](../resources/message.md) | <span data-ttu-id="16131-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="16131-140">Mail.Read</span></span> | <span data-ttu-id="16131-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="16131-141">Mail.Read</span></span> | <span data-ttu-id="16131-142">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="16131-142">Mail.Read</span></span> |
|[<span data-ttu-id="16131-143">Sicherheitswarnung</span><span class="sxs-lookup"><span data-stu-id="16131-143">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="16131-144">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16131-144">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="16131-145">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16131-145">Not supported</span></span> | <span data-ttu-id="16131-146">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16131-146">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="16131-147">user</span><span class="sxs-lookup"><span data-stu-id="16131-147">user</span></span>](../resources/user.md) | <span data-ttu-id="16131-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="16131-148">User.Read.All</span></span> | <span data-ttu-id="16131-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="16131-149">User.Read.All</span></span> | <span data-ttu-id="16131-150">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="16131-150">User.Read.All</span></span> |

> <span data-ttu-id="16131-151">**Hinweis:** Es gibt zusätzliche Einschränkungen für Abonnements für OneDrive-und Outlook-Elemente.</span><span class="sxs-lookup"><span data-stu-id="16131-151">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="16131-152">Die Einschränkungen gelten für das Erstellen und Verwalten von Abonnements (erhalten, aktualisieren und Löschen von Abonnements).</span><span class="sxs-lookup"><span data-stu-id="16131-152">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="16131-153">In persönlichen OneDrive können Sie den Stammordner oder einen beliebigen Unterordner in diesem Laufwerk abonnieren.</span><span class="sxs-lookup"><span data-stu-id="16131-153">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="16131-154">In OneDrive for Business können Sie nur den Stammordner abonnieren.</span><span class="sxs-lookup"><span data-stu-id="16131-154">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="16131-155">Benachrichtigungen werden für die angeforderten Arten von Änderungen im abonnierten Ordner oder in einer beliebigen Datei, einem Ordner oder einem anderen driveItem-Objekt in der Hierarchie gesendet.</span><span class="sxs-lookup"><span data-stu-id="16131-155">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="16131-156">Sie können keine **Laufwerks** -oder **driveItem** -Instanzen abonnieren, die keine Ordner sind, wie beispielsweise einzelne Dateien.</span><span class="sxs-lookup"><span data-stu-id="16131-156">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="16131-157">In Outlook unterstützt die Delegierte Berechtigung das Abonnieren von Elementen in Ordnern nur im Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="16131-157">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="16131-158">Das kann beispielsweise nicht die Delegierte Berechtigung Calendars. Read verwenden, um Ereignisse im Postfach eines anderen Benutzers zu abonnieren.</span><span class="sxs-lookup"><span data-stu-id="16131-158">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="16131-159">So abonnieren Sie Änderungsbenachrichtigungen für Outlook-Kontakte,-Ereignisse oder-Nachrichten in _freigegebenen oder Delegierten_ Ordnern:</span><span class="sxs-lookup"><span data-stu-id="16131-159">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="16131-160">Verwenden Sie die entsprechende Anwendungsberechtigung, um Änderungen an Elementen in einem Ordner oder Postfach eines _beliebigen_ Benutzers im Mandanten zu abonnieren.</span><span class="sxs-lookup"><span data-stu-id="16131-160">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="16131-161">Verwenden Sie nicht die Outlook-Freigabeberechtigungen (Contacts. Read. Shared, Calendars. Read. Shared, Mail. Read. Shared und ihre Pendants für Lese-/Schreibzugriff), da Sie das Abonnieren von Änderungsbenachrichtigungen für Elemente in freigegebenen oder Delegierten Ordnern **nicht** unterstützen.</span><span class="sxs-lookup"><span data-stu-id="16131-161">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="16131-162">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="16131-162">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="16131-163">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="16131-163">Request headers</span></span>

| <span data-ttu-id="16131-164">Name</span><span class="sxs-lookup"><span data-stu-id="16131-164">Name</span></span>       | <span data-ttu-id="16131-165">Typ</span><span class="sxs-lookup"><span data-stu-id="16131-165">Type</span></span> | <span data-ttu-id="16131-166">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16131-166">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="16131-167">Authorization</span><span class="sxs-lookup"><span data-stu-id="16131-167">Authorization</span></span>  | <span data-ttu-id="16131-168">string</span><span class="sxs-lookup"><span data-stu-id="16131-168">string</span></span>  | <span data-ttu-id="16131-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16131-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="16131-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="16131-171">Response</span></span>

<span data-ttu-id="16131-172">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="16131-172">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16131-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="16131-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="16131-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="16131-174">Request</span></span>

<span data-ttu-id="16131-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="16131-175">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="16131-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="16131-176">Response</span></span>

<span data-ttu-id="16131-177">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="16131-177">Here is an example of the response.</span></span>
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
