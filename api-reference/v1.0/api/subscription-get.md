---
title: Abonnement abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.
localization_priority: Priority
ms.openlocfilehash: a9cdc93d958895deaeb8778b69651a898d5a94c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840299"
---
# <a name="get-subscription"></a><span data-ttu-id="4020d-103">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="4020d-103">Get subscription</span></span>

<span data-ttu-id="4020d-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.</span><span class="sxs-lookup"><span data-stu-id="4020d-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="4020d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4020d-105">Permissions</span></span>

<span data-ttu-id="4020d-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4020d-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4020d-108">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="4020d-108">Resource type / Item</span></span>        | <span data-ttu-id="4020d-109">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="4020d-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="4020d-110">Kontakte</span><span class="sxs-lookup"><span data-stu-id="4020d-110">Contacts</span></span>                    | <span data-ttu-id="4020d-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4020d-111">Contacts.Read</span></span>       |
| <span data-ttu-id="4020d-112">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="4020d-112">Conversations</span></span>               | <span data-ttu-id="4020d-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4020d-113">Group.Read.All</span></span>      |
| <span data-ttu-id="4020d-114">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="4020d-114">Events</span></span>                      | <span data-ttu-id="4020d-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4020d-115">Calendars.Read</span></span>      |
| <span data-ttu-id="4020d-116">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4020d-116">Messages</span></span>                    | <span data-ttu-id="4020d-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4020d-117">Mail.Read</span></span>           |
| <span data-ttu-id="4020d-118">Gruppen</span><span class="sxs-lookup"><span data-stu-id="4020d-118">Groups</span></span>                      | <span data-ttu-id="4020d-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4020d-119">Group.Read.All</span></span>      |
| <span data-ttu-id="4020d-120">Benutzer</span><span class="sxs-lookup"><span data-stu-id="4020d-120">Users</span></span>                       | <span data-ttu-id="4020d-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4020d-121">User.Read.All</span></span>       |
| <span data-ttu-id="4020d-122">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="4020d-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="4020d-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4020d-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="4020d-124">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="4020d-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="4020d-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4020d-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="4020d-126">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="4020d-126">Security alert</span></span>| <span data-ttu-id="4020d-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4020d-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4020d-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4020d-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4020d-129">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4020d-129">Optional query parameters</span></span>

<span data-ttu-id="4020d-130">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4020d-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4020d-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4020d-131">Request headers</span></span>

| <span data-ttu-id="4020d-132">Name</span><span class="sxs-lookup"><span data-stu-id="4020d-132">Name</span></span>       | <span data-ttu-id="4020d-133">Typ</span><span class="sxs-lookup"><span data-stu-id="4020d-133">Type</span></span> | <span data-ttu-id="4020d-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4020d-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4020d-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="4020d-135">Authorization</span></span>  | <span data-ttu-id="4020d-136">string</span><span class="sxs-lookup"><span data-stu-id="4020d-136">string</span></span>  | <span data-ttu-id="4020d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4020d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4020d-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4020d-139">Request body</span></span>

<span data-ttu-id="4020d-140">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4020d-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4020d-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="4020d-141">Response</span></span>

<span data-ttu-id="4020d-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4020d-142">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4020d-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4020d-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4020d-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4020d-144">Request</span></span>

<span data-ttu-id="4020d-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4020d-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="4020d-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="4020d-146">Response</span></span>

<span data-ttu-id="4020d-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4020d-147">Here is an example of the response.</span></span>
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
