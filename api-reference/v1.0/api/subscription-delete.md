---
title: Abonnement löschen
description: Mit dieser API können Sie Abonnements löschen.
localization_priority: Normal
ms.openlocfilehash: a5bd1998df3a7e3a8896fa770c0dbdd72cd59940
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805593"
---
# <a name="delete-subscription"></a><span data-ttu-id="fb7a2-103">Abonnement löschen</span><span class="sxs-lookup"><span data-stu-id="fb7a2-103">Delete subscription</span></span>

<span data-ttu-id="fb7a2-104">Mit dieser API können Sie Abonnements löschen.</span><span class="sxs-lookup"><span data-stu-id="fb7a2-104">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb7a2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fb7a2-105">Permissions</span></span>

<span data-ttu-id="fb7a2-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb7a2-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb7a2-108">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="fb7a2-108">Resource type / Item</span></span>        | <span data-ttu-id="fb7a2-109">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="fb7a2-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="fb7a2-110">Kontakte</span><span class="sxs-lookup"><span data-stu-id="fb7a2-110">Contacts</span></span>                    | <span data-ttu-id="fb7a2-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fb7a2-111">Contacts.Read</span></span>       |
| <span data-ttu-id="fb7a2-112">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="fb7a2-112">Conversations</span></span>               | <span data-ttu-id="fb7a2-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb7a2-113">Group.Read.All</span></span>      |
| <span data-ttu-id="fb7a2-114">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="fb7a2-114">Events</span></span>                      | <span data-ttu-id="fb7a2-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fb7a2-115">Calendars.Read</span></span>      |
| <span data-ttu-id="fb7a2-116">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="fb7a2-116">Messages</span></span>                    | <span data-ttu-id="fb7a2-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fb7a2-117">Mail.Read</span></span>           |
| <span data-ttu-id="fb7a2-118">Gruppen</span><span class="sxs-lookup"><span data-stu-id="fb7a2-118">Groups</span></span>                      | <span data-ttu-id="fb7a2-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb7a2-119">Group.Read.All</span></span>      |
| <span data-ttu-id="fb7a2-120">Benutzer</span><span class="sxs-lookup"><span data-stu-id="fb7a2-120">Users</span></span>                       | <span data-ttu-id="fb7a2-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb7a2-121">User.Read.All</span></span>       |
| <span data-ttu-id="fb7a2-122">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="fb7a2-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="fb7a2-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb7a2-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="fb7a2-124">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="fb7a2-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="fb7a2-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb7a2-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="fb7a2-126">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="fb7a2-126">Security alert</span></span>| <span data-ttu-id="fb7a2-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb7a2-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb7a2-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb7a2-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fb7a2-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fb7a2-129">Request headers</span></span>

| <span data-ttu-id="fb7a2-130">Name</span><span class="sxs-lookup"><span data-stu-id="fb7a2-130">Name</span></span>       | <span data-ttu-id="fb7a2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="fb7a2-131">Type</span></span> | <span data-ttu-id="fb7a2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fb7a2-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fb7a2-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb7a2-133">Authorization</span></span>  | <span data-ttu-id="fb7a2-134">string</span><span class="sxs-lookup"><span data-stu-id="fb7a2-134">string</span></span>  | <span data-ttu-id="fb7a2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fb7a2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb7a2-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fb7a2-137">Request body</span></span>

<span data-ttu-id="fb7a2-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fb7a2-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb7a2-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb7a2-139">Response</span></span>

<span data-ttu-id="fb7a2-140">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fb7a2-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fb7a2-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fb7a2-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fb7a2-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb7a2-142">Request</span></span>

<span data-ttu-id="fb7a2-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fb7a2-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="fb7a2-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb7a2-144">Response</span></span>

<span data-ttu-id="fb7a2-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fb7a2-145">Here is an example of the response.</span></span>
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
