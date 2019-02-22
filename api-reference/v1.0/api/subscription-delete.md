---
title: Abonnement löschen
description: Mit dieser API können Sie Abonnements löschen.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 97df6f59d4a8acfacec479e718970feef0c77632
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161432"
---
# <a name="delete-subscription"></a><span data-ttu-id="9e273-103">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="9e273-103">Delete subscription</span></span>

<span data-ttu-id="9e273-104">Mit dieser API können Sie Abonnements löschen.</span><span class="sxs-lookup"><span data-stu-id="9e273-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e273-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9e273-105">Permissions</span></span>

<span data-ttu-id="9e273-106">Abhängig von der angeforderten Ressource und dem Berechtigungstyp (Delegierte oder Anwendung) ist die in der folgenden Tabelle angegebene Berechtigung die am wenigsten privilegierten Berechtigungen zum Aufrufen dieser API.</span><span class="sxs-lookup"><span data-stu-id="9e273-106">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="9e273-107">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e273-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e273-108">Unterstützte Ressource</span><span class="sxs-lookup"><span data-stu-id="9e273-108">Supported resource</span></span> | <span data-ttu-id="9e273-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9e273-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9e273-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9e273-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e273-111">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9e273-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="9e273-112">Kontakt</span><span class="sxs-lookup"><span data-stu-id="9e273-112">contact</span></span>](../resources/contact.md) | <span data-ttu-id="9e273-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9e273-113">Contacts.Read</span></span> | <span data-ttu-id="9e273-114">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9e273-114">Contacts.Read</span></span> | <span data-ttu-id="9e273-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9e273-115">Contacts.Read</span></span> |
|<span data-ttu-id="9e273-116">[driveItem](../resources/driveitem.md) (persönliche OneDrive des Benutzers)</span><span class="sxs-lookup"><span data-stu-id="9e273-116">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="9e273-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e273-117">Not supported</span></span> | <span data-ttu-id="9e273-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e273-118">Files.ReadWrite</span></span> | <span data-ttu-id="9e273-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e273-119">Not supported</span></span> |
|<span data-ttu-id="9e273-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="9e273-120">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="9e273-121">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e273-121">Files.ReadWrite.All</span></span> | <span data-ttu-id="9e273-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e273-122">Not supported</span></span> | <span data-ttu-id="9e273-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e273-123">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="9e273-124">event</span><span class="sxs-lookup"><span data-stu-id="9e273-124">event</span></span>](../resources/event.md) | <span data-ttu-id="9e273-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9e273-125">Calendars.Read</span></span> | <span data-ttu-id="9e273-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9e273-126">Calendars.Read</span></span> | <span data-ttu-id="9e273-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9e273-127">Calendars.Read</span></span> |
|[<span data-ttu-id="9e273-128">group</span><span class="sxs-lookup"><span data-stu-id="9e273-128">group</span></span>](../resources/group.md) | <span data-ttu-id="9e273-129">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e273-129">Group.Read.All</span></span> | <span data-ttu-id="9e273-130">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e273-130">Not supported</span></span> | <span data-ttu-id="9e273-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e273-131">Group.Read.All</span></span> |
|[<span data-ttu-id="9e273-132">Gruppenunterhaltung</span><span class="sxs-lookup"><span data-stu-id="9e273-132">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="9e273-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e273-133">Group.Read.All</span></span> | <span data-ttu-id="9e273-134">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e273-134">Not supported</span></span> | <span data-ttu-id="9e273-135">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e273-135">Not supported</span></span> |
|[<span data-ttu-id="9e273-136">Nachricht</span><span class="sxs-lookup"><span data-stu-id="9e273-136">message</span></span>](../resources/message.md) | <span data-ttu-id="9e273-137">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9e273-137">Mail.Read</span></span> | <span data-ttu-id="9e273-138">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9e273-138">Mail.Read</span></span> | <span data-ttu-id="9e273-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9e273-139">Mail.Read</span></span> |
|[<span data-ttu-id="9e273-140">Sicherheitswarnung</span><span class="sxs-lookup"><span data-stu-id="9e273-140">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="9e273-141">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e273-141">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="9e273-142">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e273-142">Not supported</span></span> | <span data-ttu-id="9e273-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e273-143">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="9e273-144">user</span><span class="sxs-lookup"><span data-stu-id="9e273-144">user</span></span>](../resources/user.md) | <span data-ttu-id="9e273-145">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e273-145">User.Read.All</span></span> | <span data-ttu-id="9e273-146">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e273-146">User.Read.All</span></span> | <span data-ttu-id="9e273-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e273-147">User.Read.All</span></span> |

> <span data-ttu-id="9e273-148">**Hinweis:** Es gibt zusätzliche Einschränkungen für Abonnements für OneDrive-und Outlook-Elemente.</span><span class="sxs-lookup"><span data-stu-id="9e273-148">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="9e273-149">Die Einschränkungen gelten für das Erstellen und Verwalten von Abonnements (erhalten, aktualisieren und Löschen von Abonnements).</span><span class="sxs-lookup"><span data-stu-id="9e273-149">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="9e273-150">In persönlichen OneDrive können Sie den Stammordner oder einen beliebigen Unterordner in diesem Laufwerk abonnieren.</span><span class="sxs-lookup"><span data-stu-id="9e273-150">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="9e273-151">In OneDrive for Business können Sie nur den Stammordner abonnieren.</span><span class="sxs-lookup"><span data-stu-id="9e273-151">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="9e273-152">Benachrichtigungen werden für die angeforderten Arten von Änderungen im abonnierten Ordner oder in einer beliebigen Datei, einem Ordner oder einem anderen driveItem-Objekt in der Hierarchie gesendet.</span><span class="sxs-lookup"><span data-stu-id="9e273-152">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other driveItem objects in its hierarchy.</span></span> <span data-ttu-id="9e273-153">Sie können keine **Laufwerks** -oder **driveItem** -Instanzen abonnieren, die keine Ordner sind, wie beispielsweise einzelne Dateien.</span><span class="sxs-lookup"><span data-stu-id="9e273-153">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="9e273-154">In Outlook unterstützt die Delegierte Berechtigung das Abonnieren von Elementen in Ordnern nur im Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="9e273-154">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="9e273-155">Das kann beispielsweise nicht die Delegierte Berechtigung Calendars. Read verwenden, um Ereignisse im Postfach eines anderen Benutzers zu abonnieren.</span><span class="sxs-lookup"><span data-stu-id="9e273-155">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="9e273-156">So abonnieren Sie Änderungsbenachrichtigungen für Outlook-Kontakte,-Ereignisse oder-Nachrichten in _freigegebenen oder Delegierten_ Ordnern:</span><span class="sxs-lookup"><span data-stu-id="9e273-156">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="9e273-157">Verwenden Sie die entsprechende Anwendungsberechtigung, um Änderungen an Elementen in einem Ordner oder Postfach eines _beliebigen_ Benutzers im Mandanten zu abonnieren.</span><span class="sxs-lookup"><span data-stu-id="9e273-157">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="9e273-158">Verwenden Sie nicht die Outlook-Freigabeberechtigungen (Contacts. Read. Shared, Calendars. Read. Shared, Mail. Read. Shared und ihre Pendants für Lese-/Schreibzugriff), da Sie das Abonnieren von Änderungsbenachrichtigungen für Elemente in freigegebenen oder Delegierten Ordnern **nicht** unterstützen.</span><span class="sxs-lookup"><span data-stu-id="9e273-158">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="9e273-159">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e273-159">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9e273-160">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9e273-160">Request headers</span></span>

| <span data-ttu-id="9e273-161">Name</span><span class="sxs-lookup"><span data-stu-id="9e273-161">Name</span></span>       | <span data-ttu-id="9e273-162">Typ</span><span class="sxs-lookup"><span data-stu-id="9e273-162">Type</span></span> | <span data-ttu-id="9e273-163">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e273-163">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9e273-164">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e273-164">Authorization</span></span>  | <span data-ttu-id="9e273-165">string</span><span class="sxs-lookup"><span data-stu-id="9e273-165">string</span></span>  | <span data-ttu-id="9e273-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9e273-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e273-168">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9e273-168">Request body</span></span>

<span data-ttu-id="9e273-169">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9e273-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e273-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e273-170">Response</span></span>

<span data-ttu-id="9e273-171">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e273-171">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9e273-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9e273-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9e273-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e273-173">Request</span></span>

<span data-ttu-id="9e273-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9e273-174">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="9e273-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e273-175">Response</span></span>

<span data-ttu-id="9e273-176">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9e273-176">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
