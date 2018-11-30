---
title: Abonnement löschen
description: Mit dieser API können Sie Abonnements löschen.
ms.openlocfilehash: 249393cef11e2768eec0a6435a8485b51cf6921c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019898"
---
# <a name="delete-subscription"></a><span data-ttu-id="56402-103">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="56402-103">Delete subscription</span></span>

<span data-ttu-id="56402-104">Mit dieser API können Sie Abonnements löschen.</span><span class="sxs-lookup"><span data-stu-id="56402-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="56402-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="56402-105">Permissions</span></span>

<span data-ttu-id="56402-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56402-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56402-108">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="56402-108">Resource type / Item</span></span>        | <span data-ttu-id="56402-109">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="56402-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="56402-110">Kontakte</span><span class="sxs-lookup"><span data-stu-id="56402-110">Contacts</span></span>                    | <span data-ttu-id="56402-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="56402-111">Contacts.Read</span></span>       |
| <span data-ttu-id="56402-112">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="56402-112">Conversations</span></span>               | <span data-ttu-id="56402-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="56402-113">Group.Read.All</span></span>      |
| <span data-ttu-id="56402-114">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="56402-114">Events</span></span>                      | <span data-ttu-id="56402-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="56402-115">Calendars.Read</span></span>      |
| <span data-ttu-id="56402-116">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="56402-116">Messages</span></span>                    | <span data-ttu-id="56402-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="56402-117">Mail.Read</span></span>           |
| <span data-ttu-id="56402-118">Gruppen</span><span class="sxs-lookup"><span data-stu-id="56402-118">Groups</span></span>                      | <span data-ttu-id="56402-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="56402-119">Group.Read.All</span></span>      |
| <span data-ttu-id="56402-120">Benutzer</span><span class="sxs-lookup"><span data-stu-id="56402-120">Users</span></span>                       | <span data-ttu-id="56402-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="56402-121">User.Read.All</span></span>       |
| <span data-ttu-id="56402-122">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="56402-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="56402-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56402-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="56402-124">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="56402-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="56402-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56402-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="56402-126">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="56402-126">Security alert</span></span>| <span data-ttu-id="56402-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56402-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56402-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56402-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="56402-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56402-129">Request headers</span></span>

| <span data-ttu-id="56402-130">Name</span><span class="sxs-lookup"><span data-stu-id="56402-130">Name</span></span>       | <span data-ttu-id="56402-131">Typ</span><span class="sxs-lookup"><span data-stu-id="56402-131">Type</span></span> | <span data-ttu-id="56402-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56402-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="56402-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="56402-133">Authorization</span></span>  | <span data-ttu-id="56402-134">string</span><span class="sxs-lookup"><span data-stu-id="56402-134">string</span></span>  | <span data-ttu-id="56402-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="56402-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56402-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56402-137">Request body</span></span>

<span data-ttu-id="56402-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="56402-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56402-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="56402-139">Response</span></span>

<span data-ttu-id="56402-140">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56402-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="56402-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56402-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="56402-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56402-142">Request</span></span>

<span data-ttu-id="56402-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56402-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="56402-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="56402-144">Response</span></span>

<span data-ttu-id="56402-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="56402-145">Here is an example of the response.</span></span>
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
