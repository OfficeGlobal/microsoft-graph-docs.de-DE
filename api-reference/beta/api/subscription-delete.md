---
title: Abonnement löschen
description: Mit dieser API können Sie Abonnements löschen.
localization_priority: Normal
ms.openlocfilehash: 1e2efb9835e5e625bdac0385b5011cfe5c8c64b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842049"
---
# <a name="delete-subscription"></a><span data-ttu-id="b1863-103">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="b1863-103">Delete subscription</span></span>

> <span data-ttu-id="b1863-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b1863-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1863-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1863-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1863-106">Mit dieser API können Sie Abonnements löschen.</span><span class="sxs-lookup"><span data-stu-id="b1863-106">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1863-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b1863-107">Permissions</span></span>

<span data-ttu-id="b1863-p102">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1863-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1863-110">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="b1863-110">Resource type / Item</span></span>        | <span data-ttu-id="b1863-111">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="b1863-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="b1863-112">Kontakte</span><span class="sxs-lookup"><span data-stu-id="b1863-112">Contacts</span></span>                    | <span data-ttu-id="b1863-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b1863-113">Contacts.Read</span></span>       |
| <span data-ttu-id="b1863-114">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="b1863-114">Conversations</span></span>               | <span data-ttu-id="b1863-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1863-115">Group.Read.All</span></span>      |
| <span data-ttu-id="b1863-116">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="b1863-116">Events</span></span>                      | <span data-ttu-id="b1863-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b1863-117">Calendars.Read</span></span>      |
| <span data-ttu-id="b1863-118">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="b1863-118">Messages</span></span>                    | <span data-ttu-id="b1863-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b1863-119">Mail.Read</span></span>           |
| <span data-ttu-id="b1863-120">Gruppen</span><span class="sxs-lookup"><span data-stu-id="b1863-120">Groups</span></span>                      | <span data-ttu-id="b1863-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1863-121">Group.Read.All</span></span>      |
| <span data-ttu-id="b1863-122">Benutzer</span><span class="sxs-lookup"><span data-stu-id="b1863-122">Users</span></span>                       | <span data-ttu-id="b1863-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1863-123">User.Read.All</span></span>       |
| <span data-ttu-id="b1863-124">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="b1863-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="b1863-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1863-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="b1863-126">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="b1863-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="b1863-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1863-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="b1863-128">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="b1863-128">Security alert</span></span>              | <span data-ttu-id="b1863-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1863-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="b1863-130">***Hinweis:*** Der Endpunkt /beta kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="b1863-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="b1863-131">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1863-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="b1863-132">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1863-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b1863-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1863-133">Request headers</span></span>

| <span data-ttu-id="b1863-134">Name</span><span class="sxs-lookup"><span data-stu-id="b1863-134">Name</span></span>       | <span data-ttu-id="b1863-135">Typ</span><span class="sxs-lookup"><span data-stu-id="b1863-135">Type</span></span> | <span data-ttu-id="b1863-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1863-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1863-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1863-137">Authorization</span></span>  | <span data-ttu-id="b1863-138">string</span><span class="sxs-lookup"><span data-stu-id="b1863-138">string</span></span>  | <span data-ttu-id="b1863-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b1863-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1863-141">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1863-141">Request body</span></span>

<span data-ttu-id="b1863-142">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b1863-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1863-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1863-143">Response</span></span>

<span data-ttu-id="b1863-144">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1863-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b1863-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1863-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b1863-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1863-146">Request</span></span>

<span data-ttu-id="b1863-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1863-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="b1863-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1863-148">Response</span></span>

<span data-ttu-id="b1863-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b1863-149">Here is an example of the response.</span></span>
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
