---
title: Abonnement löschen
description: Mit dieser API können Sie Abonnements löschen.
ms.openlocfilehash: be2c32f0915e8718203e46489be9861bf0f05451
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059732"
---
# <a name="delete-subscription"></a><span data-ttu-id="6a187-103">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="6a187-103">Delete subscription</span></span>

> <span data-ttu-id="6a187-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6a187-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a187-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a187-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a187-106">Mit dieser API können Sie Abonnements löschen.</span><span class="sxs-lookup"><span data-stu-id="6a187-106">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a187-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6a187-107">Permissions</span></span>

<span data-ttu-id="6a187-p102">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a187-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a187-110">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="6a187-110">Resource type / Item</span></span>        | <span data-ttu-id="6a187-111">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="6a187-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="6a187-112">Kontakte</span><span class="sxs-lookup"><span data-stu-id="6a187-112">Contacts</span></span>                    | <span data-ttu-id="6a187-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6a187-113">Contacts.Read</span></span>       |
| <span data-ttu-id="6a187-114">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="6a187-114">Conversations</span></span>               | <span data-ttu-id="6a187-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a187-115">Group.Read.All</span></span>      |
| <span data-ttu-id="6a187-116">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="6a187-116">Events</span></span>                      | <span data-ttu-id="6a187-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6a187-117">Calendars.Read</span></span>      |
| <span data-ttu-id="6a187-118">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="6a187-118">Messages</span></span>                    | <span data-ttu-id="6a187-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6a187-119">Mail.Read</span></span>           |
| <span data-ttu-id="6a187-120">Gruppen</span><span class="sxs-lookup"><span data-stu-id="6a187-120">Groups</span></span>                      | <span data-ttu-id="6a187-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a187-121">Group.Read.All</span></span>      |
| <span data-ttu-id="6a187-122">Benutzer</span><span class="sxs-lookup"><span data-stu-id="6a187-122">Users</span></span>                       | <span data-ttu-id="6a187-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a187-123">User.Read.All</span></span>       |
| <span data-ttu-id="6a187-124">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="6a187-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="6a187-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a187-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="6a187-126">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="6a187-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="6a187-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a187-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="6a187-128">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="6a187-128">Security alert</span></span>              | <span data-ttu-id="6a187-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a187-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="6a187-130">***Hinweis:*** Der Endpunkt /beta kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="6a187-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="6a187-131">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a187-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="6a187-132">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a187-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6a187-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a187-133">Request headers</span></span>

| <span data-ttu-id="6a187-134">Name</span><span class="sxs-lookup"><span data-stu-id="6a187-134">Name</span></span>       | <span data-ttu-id="6a187-135">Typ</span><span class="sxs-lookup"><span data-stu-id="6a187-135">Type</span></span> | <span data-ttu-id="6a187-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a187-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a187-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a187-137">Authorization</span></span>  | <span data-ttu-id="6a187-138">string</span><span class="sxs-lookup"><span data-stu-id="6a187-138">string</span></span>  | <span data-ttu-id="6a187-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a187-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a187-141">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a187-141">Request body</span></span>

<span data-ttu-id="6a187-142">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6a187-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a187-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a187-143">Response</span></span>

<span data-ttu-id="6a187-144">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a187-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6a187-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a187-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6a187-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a187-146">Request</span></span>

<span data-ttu-id="6a187-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a187-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="6a187-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a187-148">Response</span></span>

<span data-ttu-id="6a187-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6a187-149">Here is an example of the response.</span></span>
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
