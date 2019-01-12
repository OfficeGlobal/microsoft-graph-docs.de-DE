---
title: Abonnement löschen
description: Mit dieser API können Sie Abonnements löschen.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 79ffce638036414469953d6d729229e00cb1662f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945874"
---
# <a name="delete-subscription"></a><span data-ttu-id="b1bb6-103">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="b1bb6-103">Delete subscription</span></span>

> <span data-ttu-id="b1bb6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b1bb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1bb6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1bb6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1bb6-106">Mit dieser API können Sie Abonnements löschen.</span><span class="sxs-lookup"><span data-stu-id="b1bb6-106">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1bb6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b1bb6-107">Permissions</span></span>

<span data-ttu-id="b1bb6-p102">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1bb6-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1bb6-110">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="b1bb6-110">Resource type / Item</span></span>        | <span data-ttu-id="b1bb6-111">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="b1bb6-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="b1bb6-112">Kontakte</span><span class="sxs-lookup"><span data-stu-id="b1bb6-112">Contacts</span></span>                    | <span data-ttu-id="b1bb6-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b1bb6-113">Contacts.Read</span></span>       |
| <span data-ttu-id="b1bb6-114">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="b1bb6-114">Conversations</span></span>               | <span data-ttu-id="b1bb6-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1bb6-115">Group.Read.All</span></span>      |
| <span data-ttu-id="b1bb6-116">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="b1bb6-116">Events</span></span>                      | <span data-ttu-id="b1bb6-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b1bb6-117">Calendars.Read</span></span>      |
| <span data-ttu-id="b1bb6-118">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="b1bb6-118">Messages</span></span>                    | <span data-ttu-id="b1bb6-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b1bb6-119">Mail.Read</span></span>           |
| <span data-ttu-id="b1bb6-120">Gruppen</span><span class="sxs-lookup"><span data-stu-id="b1bb6-120">Groups</span></span>                      | <span data-ttu-id="b1bb6-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1bb6-121">Group.Read.All</span></span>      |
| <span data-ttu-id="b1bb6-122">Benutzer</span><span class="sxs-lookup"><span data-stu-id="b1bb6-122">Users</span></span>                       | <span data-ttu-id="b1bb6-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1bb6-123">User.Read.All</span></span>       |
| <span data-ttu-id="b1bb6-124">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="b1bb6-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="b1bb6-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1bb6-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="b1bb6-126">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="b1bb6-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="b1bb6-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1bb6-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="b1bb6-128">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="b1bb6-128">Security alert</span></span>              | <span data-ttu-id="b1bb6-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1bb6-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="b1bb6-130">***Hinweis:*** Der Endpunkt /beta kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="b1bb6-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="b1bb6-131">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1bb6-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="b1bb6-132">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1bb6-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b1bb6-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1bb6-133">Request headers</span></span>

| <span data-ttu-id="b1bb6-134">Name</span><span class="sxs-lookup"><span data-stu-id="b1bb6-134">Name</span></span>       | <span data-ttu-id="b1bb6-135">Typ</span><span class="sxs-lookup"><span data-stu-id="b1bb6-135">Type</span></span> | <span data-ttu-id="b1bb6-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1bb6-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1bb6-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1bb6-137">Authorization</span></span>  | <span data-ttu-id="b1bb6-138">string</span><span class="sxs-lookup"><span data-stu-id="b1bb6-138">string</span></span>  | <span data-ttu-id="b1bb6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b1bb6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1bb6-141">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1bb6-141">Request body</span></span>

<span data-ttu-id="b1bb6-142">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b1bb6-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1bb6-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1bb6-143">Response</span></span>

<span data-ttu-id="b1bb6-144">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1bb6-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b1bb6-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1bb6-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b1bb6-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1bb6-146">Request</span></span>

<span data-ttu-id="b1bb6-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1bb6-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="b1bb6-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1bb6-148">Response</span></span>

<span data-ttu-id="b1bb6-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b1bb6-149">Here is an example of the response.</span></span>
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
