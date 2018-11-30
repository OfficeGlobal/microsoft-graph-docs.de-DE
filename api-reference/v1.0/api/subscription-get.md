---
title: Abonnement abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.
ms.openlocfilehash: 62bcb730a5743146113cda30d6dafa022afa4fc1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017469"
---
# <a name="get-subscription"></a><span data-ttu-id="2027a-103">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="2027a-103">Get subscription</span></span>

<span data-ttu-id="2027a-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.</span><span class="sxs-lookup"><span data-stu-id="2027a-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="2027a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2027a-105">Permissions</span></span>

<span data-ttu-id="2027a-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2027a-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2027a-108">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="2027a-108">Resource type / Item</span></span>        | <span data-ttu-id="2027a-109">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="2027a-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="2027a-110">Kontakte</span><span class="sxs-lookup"><span data-stu-id="2027a-110">Contacts</span></span>                    | <span data-ttu-id="2027a-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2027a-111">Contacts.Read</span></span>       |
| <span data-ttu-id="2027a-112">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="2027a-112">Conversations</span></span>               | <span data-ttu-id="2027a-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2027a-113">Group.Read.All</span></span>      |
| <span data-ttu-id="2027a-114">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="2027a-114">Events</span></span>                      | <span data-ttu-id="2027a-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2027a-115">Calendars.Read</span></span>      |
| <span data-ttu-id="2027a-116">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="2027a-116">Messages</span></span>                    | <span data-ttu-id="2027a-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2027a-117">Mail.Read</span></span>           |
| <span data-ttu-id="2027a-118">Gruppen</span><span class="sxs-lookup"><span data-stu-id="2027a-118">Groups</span></span>                      | <span data-ttu-id="2027a-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2027a-119">Group.Read.All</span></span>      |
| <span data-ttu-id="2027a-120">Benutzer</span><span class="sxs-lookup"><span data-stu-id="2027a-120">Users</span></span>                       | <span data-ttu-id="2027a-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2027a-121">User.Read.All</span></span>       |
| <span data-ttu-id="2027a-122">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="2027a-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="2027a-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2027a-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="2027a-124">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="2027a-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="2027a-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2027a-125">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="2027a-126">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="2027a-126">Security alert</span></span>| <span data-ttu-id="2027a-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2027a-127">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2027a-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2027a-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2027a-129">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2027a-129">Optional query parameters</span></span>

<span data-ttu-id="2027a-130">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2027a-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2027a-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2027a-131">Request headers</span></span>

| <span data-ttu-id="2027a-132">Name</span><span class="sxs-lookup"><span data-stu-id="2027a-132">Name</span></span>       | <span data-ttu-id="2027a-133">Typ</span><span class="sxs-lookup"><span data-stu-id="2027a-133">Type</span></span> | <span data-ttu-id="2027a-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2027a-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2027a-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="2027a-135">Authorization</span></span>  | <span data-ttu-id="2027a-136">string</span><span class="sxs-lookup"><span data-stu-id="2027a-136">string</span></span>  | <span data-ttu-id="2027a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2027a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2027a-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2027a-139">Request body</span></span>

<span data-ttu-id="2027a-140">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2027a-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2027a-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2027a-141">Response</span></span>

<span data-ttu-id="2027a-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2027a-142">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2027a-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2027a-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2027a-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2027a-144">Request</span></span>

<span data-ttu-id="2027a-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2027a-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="2027a-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="2027a-146">Response</span></span>

<span data-ttu-id="2027a-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2027a-147">Here is an example of the response.</span></span>
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
