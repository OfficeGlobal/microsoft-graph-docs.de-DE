---
title: Abonnement abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c73f01a65a2b81bfa34818f9a7a96f754501bd65
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163469"
---
# <a name="get-subscription"></a><span data-ttu-id="73ae3-103">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="73ae3-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73ae3-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.</span><span class="sxs-lookup"><span data-stu-id="73ae3-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="73ae3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="73ae3-105">Permissions</span></span>

<span data-ttu-id="73ae3-106">Abhängig von der angeforderten Ressource und dem Berechtigungstyp (Delegierte oder Anwendung) ist die in der folgenden Tabelle angegebene Berechtigung die am wenigsten privilegierten Berechtigungen zum Aufrufen dieser API.</span><span class="sxs-lookup"><span data-stu-id="73ae3-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="73ae3-107">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73ae3-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73ae3-108">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="73ae3-108">Supported resource</span></span> | <span data-ttu-id="73ae3-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73ae3-109">Delegated (work or school account)</span></span> | <span data-ttu-id="73ae3-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73ae3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73ae3-111">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73ae3-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="73ae3-112">Kontakt</span><span class="sxs-lookup"><span data-stu-id="73ae3-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="73ae3-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73ae3-113">Contacts.Read</span></span> | <span data-ttu-id="73ae3-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73ae3-114">Contacts.Read</span></span> | <span data-ttu-id="73ae3-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73ae3-115">Contacts.Read</span></span> |
|<span data-ttu-id="73ae3-116">[driveItem](../resources/driveitem.md) (persönliche OneDrive des Benutzers)</span><span class="sxs-lookup"><span data-stu-id="73ae3-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="73ae3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73ae3-117">Not supported</span></span> | <span data-ttu-id="73ae3-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73ae3-118">Files.ReadWrite</span></span> | <span data-ttu-id="73ae3-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73ae3-119">Not supported</span></span> |
|<span data-ttu-id="73ae3-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="73ae3-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="73ae3-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73ae3-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="73ae3-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73ae3-122">Not supported</span></span> | <span data-ttu-id="73ae3-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73ae3-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="73ae3-124">event</span><span class="sxs-lookup"><span data-stu-id="73ae3-124">event</span></span>](../resources/event.md) | <span data-ttu-id="73ae3-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73ae3-125">Calendars.Read</span></span> | <span data-ttu-id="73ae3-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73ae3-126">Calendars.Read</span></span> | <span data-ttu-id="73ae3-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73ae3-127">Calendars.Read</span></span> |
|[<span data-ttu-id="73ae3-128">group</span><span class="sxs-lookup"><span data-stu-id="73ae3-128">group</span></span>](../resources/group.md) | <span data-ttu-id="73ae3-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="73ae3-129">Group.Read.All</span></span> | <span data-ttu-id="73ae3-130">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73ae3-130">Not supported</span></span> | <span data-ttu-id="73ae3-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="73ae3-131">Group.Read.All</span></span> |
|[<span data-ttu-id="73ae3-132">Gruppenunterhaltung</span><span class="sxs-lookup"><span data-stu-id="73ae3-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="73ae3-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="73ae3-133">Group.Read.All</span></span> | <span data-ttu-id="73ae3-134">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73ae3-134">Not supported</span></span> | <span data-ttu-id="73ae3-135">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73ae3-135">Not supported</span></span> |
|[<span data-ttu-id="73ae3-136">Nachricht</span><span class="sxs-lookup"><span data-stu-id="73ae3-136">message</span></span>](../resources/message.md) | <span data-ttu-id="73ae3-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73ae3-137">Mail.Read</span></span> | <span data-ttu-id="73ae3-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73ae3-138">Mail.Read</span></span> | <span data-ttu-id="73ae3-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73ae3-139">Mail.Read</span></span> |
|[<span data-ttu-id="73ae3-140">Sicherheitswarnung</span><span class="sxs-lookup"><span data-stu-id="73ae3-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="73ae3-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73ae3-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="73ae3-142">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73ae3-142">Not supported</span></span> | <span data-ttu-id="73ae3-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73ae3-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="73ae3-144">user</span><span class="sxs-lookup"><span data-stu-id="73ae3-144">user</span></span>](../resources/user.md) | <span data-ttu-id="73ae3-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="73ae3-145">User.Read.All</span></span> | <span data-ttu-id="73ae3-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="73ae3-146">User.Read.All</span></span> | <span data-ttu-id="73ae3-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="73ae3-147">User.Read.All</span></span> |

> <span data-ttu-id="73ae3-148">**Hinweis:** Es gibt zusätzliche Einschränkungen für Abonnements für OneDrive-und Outlook-Elemente.</span><span class="sxs-lookup"><span data-stu-id="73ae3-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="73ae3-149">Die Einschränkungen gelten für das Erstellen und Verwalten von Abonnements (erhalten, aktualisieren und Löschen von Abonnements).</span><span class="sxs-lookup"><span data-stu-id="73ae3-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="73ae3-150">In persönlichen OneDrive können Sie den Stammordner oder einen beliebigen Unterordner in diesem Laufwerk abonnieren.</span><span class="sxs-lookup"><span data-stu-id="73ae3-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="73ae3-151">In OneDrive for Business können Sie nur den Stammordner abonnieren.</span><span class="sxs-lookup"><span data-stu-id="73ae3-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="73ae3-152">Benachrichtigungen werden für die angeforderten Arten von Änderungen im abonnierten Ordner oder in einer beliebigen Datei, einem Ordner oder einem anderen driveItem-Objekt in der Hierarchie gesendet.</span><span class="sxs-lookup"><span data-stu-id="73ae3-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="73ae3-153">Sie können keine **Laufwerks** -oder **driveItem** -Instanzen abonnieren, die keine Ordner sind, wie beispielsweise einzelne Dateien.</span><span class="sxs-lookup"><span data-stu-id="73ae3-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="73ae3-154">In Outlook unterstützt die Delegierte Berechtigung das Abonnieren von Elementen in Ordnern nur im Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="73ae3-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="73ae3-155">Das kann beispielsweise nicht die Delegierte Berechtigung Calendars. Read verwenden, um Ereignisse im Postfach eines anderen Benutzers zu abonnieren.</span><span class="sxs-lookup"><span data-stu-id="73ae3-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="73ae3-156">So abonnieren Sie Änderungsbenachrichtigungen für Outlook-Kontakte,-Ereignisse oder-Nachrichten in _freigegebenen oder Delegierten_ Ordnern:</span><span class="sxs-lookup"><span data-stu-id="73ae3-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="73ae3-157">Verwenden Sie die entsprechende Anwendungsberechtigung, um Änderungen an Elementen in einem Ordner oder Postfach eines _beliebigen_ Benutzers im Mandanten zu abonnieren.</span><span class="sxs-lookup"><span data-stu-id="73ae3-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="73ae3-158">Verwenden Sie nicht die Outlook-Freigabeberechtigungen (Contacts. Read. Shared, Calendars. Read. Shared, Mail. Read. Shared und ihre Pendants für Lese-/Schreibzugriff), da Sie das Abonnieren von Änderungsbenachrichtigungen für Elemente in freigegebenen oder Delegierten Ordnern **nicht** unterstützen.</span><span class="sxs-lookup"><span data-stu-id="73ae3-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="73ae3-159">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73ae3-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73ae3-160">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="73ae3-160">Optional query parameters</span></span>

<span data-ttu-id="73ae3-161">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="73ae3-161">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73ae3-162">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73ae3-162">Request headers</span></span>

| <span data-ttu-id="73ae3-163">Name</span><span class="sxs-lookup"><span data-stu-id="73ae3-163">Name</span></span>       | <span data-ttu-id="73ae3-164">Typ</span><span class="sxs-lookup"><span data-stu-id="73ae3-164">Type</span></span> | <span data-ttu-id="73ae3-165">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73ae3-165">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="73ae3-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="73ae3-166">Authorization</span></span>  | <span data-ttu-id="73ae3-167">string</span><span class="sxs-lookup"><span data-stu-id="73ae3-167">string</span></span>  | <span data-ttu-id="73ae3-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="73ae3-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73ae3-170">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73ae3-170">Request body</span></span>

<span data-ttu-id="73ae3-171">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="73ae3-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73ae3-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="73ae3-172">Response</span></span>

<span data-ttu-id="73ae3-173">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73ae3-173">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73ae3-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73ae3-174">Example</span></span>

##### <a name="request"></a><span data-ttu-id="73ae3-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73ae3-175">Request</span></span>

<span data-ttu-id="73ae3-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73ae3-176">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="73ae3-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="73ae3-177">Response</span></span>

<span data-ttu-id="73ae3-178">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="73ae3-178">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
