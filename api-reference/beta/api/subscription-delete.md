---
title: Abonnement löschen
description: Mit dieser API können Sie Abonnements löschen.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9ca4c772cb6d7de088550a16262275b4c43fb9c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509462"
---
# <a name="delete-subscription"></a><span data-ttu-id="d9d52-103">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="d9d52-103">Delete subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9d52-104">Mit dieser API können Sie Abonnements löschen.</span><span class="sxs-lookup"><span data-stu-id="d9d52-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9d52-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d9d52-105">Permissions</span></span>

<span data-ttu-id="d9d52-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9d52-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d9d52-108">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="d9d52-108">Resource type / Item</span></span>        | <span data-ttu-id="d9d52-109">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="d9d52-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="d9d52-110">Kontakte</span><span class="sxs-lookup"><span data-stu-id="d9d52-110">Contacts</span></span>                    | <span data-ttu-id="d9d52-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d9d52-111">Contacts.Read</span></span>       |
| <span data-ttu-id="d9d52-112">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="d9d52-112">Conversations</span></span>               | <span data-ttu-id="d9d52-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9d52-113">Group.Read.All</span></span>      |
| <span data-ttu-id="d9d52-114">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="d9d52-114">Events</span></span>                      | <span data-ttu-id="d9d52-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="d9d52-115">Calendars.Read</span></span>      |
| <span data-ttu-id="d9d52-116">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="d9d52-116">Messages</span></span>                    | <span data-ttu-id="d9d52-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d9d52-117">Mail.Read</span></span>           |
| <span data-ttu-id="d9d52-118">Gruppen</span><span class="sxs-lookup"><span data-stu-id="d9d52-118">Groups</span></span>                      | <span data-ttu-id="d9d52-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9d52-119">Group.Read.All</span></span>      |
| <span data-ttu-id="d9d52-120">Benutzer</span><span class="sxs-lookup"><span data-stu-id="d9d52-120">Users</span></span>                       | <span data-ttu-id="d9d52-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9d52-121">User.Read.All</span></span>       |
| <span data-ttu-id="d9d52-122">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="d9d52-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="d9d52-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9d52-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="d9d52-124">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="d9d52-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="d9d52-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9d52-125">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="d9d52-126">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="d9d52-126">Security alert</span></span>              | <span data-ttu-id="d9d52-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9d52-127">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="d9d52-128">***Hinweis:*** Der Endpunkt /beta kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="d9d52-128">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="d9d52-129">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9d52-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="d9d52-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9d52-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d9d52-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9d52-131">Request headers</span></span>

| <span data-ttu-id="d9d52-132">Name</span><span class="sxs-lookup"><span data-stu-id="d9d52-132">Name</span></span>       | <span data-ttu-id="d9d52-133">Typ</span><span class="sxs-lookup"><span data-stu-id="d9d52-133">Type</span></span> | <span data-ttu-id="d9d52-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9d52-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d9d52-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9d52-135">Authorization</span></span>  | <span data-ttu-id="d9d52-136">string</span><span class="sxs-lookup"><span data-stu-id="d9d52-136">string</span></span>  | <span data-ttu-id="d9d52-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d9d52-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9d52-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9d52-139">Request body</span></span>

<span data-ttu-id="d9d52-140">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d9d52-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9d52-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9d52-141">Response</span></span>

<span data-ttu-id="d9d52-142">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9d52-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d9d52-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9d52-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d9d52-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9d52-144">Request</span></span>

<span data-ttu-id="d9d52-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9d52-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="d9d52-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9d52-146">Response</span></span>

<span data-ttu-id="d9d52-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d9d52-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
