---
title: Abonnement abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 4c55c81fdb26bb706ad270e5d53ded712ea69b22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956976"
---
# <a name="get-subscription"></a><span data-ttu-id="bed4a-103">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="bed4a-103">Get subscription</span></span>

<span data-ttu-id="bed4a-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.</span><span class="sxs-lookup"><span data-stu-id="bed4a-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="bed4a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bed4a-105">Permissions</span></span>

<span data-ttu-id="bed4a-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bed4a-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bed4a-108">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="bed4a-108">Resource type / Item</span></span>        | <span data-ttu-id="bed4a-109">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="bed4a-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="bed4a-110">Kontakte</span><span class="sxs-lookup"><span data-stu-id="bed4a-110">Contacts</span></span>                    | <span data-ttu-id="bed4a-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="bed4a-111">Contacts.Read</span></span>       |
| <span data-ttu-id="bed4a-112">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="bed4a-112">Conversations</span></span>               | <span data-ttu-id="bed4a-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bed4a-113">Group.Read.All</span></span>      |
| <span data-ttu-id="bed4a-114">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="bed4a-114">Events</span></span>                      | <span data-ttu-id="bed4a-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bed4a-115">Calendars.Read</span></span>      |
| <span data-ttu-id="bed4a-116">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="bed4a-116">Messages</span></span>                    | <span data-ttu-id="bed4a-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bed4a-117">Mail.Read</span></span>           |
| <span data-ttu-id="bed4a-118">Gruppen</span><span class="sxs-lookup"><span data-stu-id="bed4a-118">Groups</span></span>                      | <span data-ttu-id="bed4a-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bed4a-119">Group.Read.All</span></span>      |
| <span data-ttu-id="bed4a-120">Benutzer</span><span class="sxs-lookup"><span data-stu-id="bed4a-120">Users</span></span>                       | <span data-ttu-id="bed4a-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bed4a-121">User.Read.All</span></span>       |
| <span data-ttu-id="bed4a-122">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="bed4a-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="bed4a-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bed4a-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="bed4a-124">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="bed4a-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="bed4a-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bed4a-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="bed4a-126">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="bed4a-126">Security alert</span></span>| <span data-ttu-id="bed4a-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bed4a-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bed4a-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bed4a-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bed4a-129">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bed4a-129">Optional query parameters</span></span>

<span data-ttu-id="bed4a-130">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bed4a-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bed4a-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bed4a-131">Request headers</span></span>

| <span data-ttu-id="bed4a-132">Name</span><span class="sxs-lookup"><span data-stu-id="bed4a-132">Name</span></span>       | <span data-ttu-id="bed4a-133">Typ</span><span class="sxs-lookup"><span data-stu-id="bed4a-133">Type</span></span> | <span data-ttu-id="bed4a-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bed4a-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bed4a-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="bed4a-135">Authorization</span></span>  | <span data-ttu-id="bed4a-136">string</span><span class="sxs-lookup"><span data-stu-id="bed4a-136">string</span></span>  | <span data-ttu-id="bed4a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bed4a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bed4a-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bed4a-139">Request body</span></span>

<span data-ttu-id="bed4a-140">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bed4a-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bed4a-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="bed4a-141">Response</span></span>

<span data-ttu-id="bed4a-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bed4a-142">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bed4a-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bed4a-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bed4a-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bed4a-144">Request</span></span>

<span data-ttu-id="bed4a-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bed4a-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="bed4a-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="bed4a-146">Response</span></span>

<span data-ttu-id="bed4a-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bed4a-147">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
