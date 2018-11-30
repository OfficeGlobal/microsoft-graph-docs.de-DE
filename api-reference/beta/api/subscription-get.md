---
title: Abonnement abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.
ms.openlocfilehash: 5694015fe7e8cbf87b5d62f7ae4af35d1773532b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061330"
---
# <a name="get-subscription"></a><span data-ttu-id="43db2-103">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="43db2-103">Get subscription</span></span>

> <span data-ttu-id="43db2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="43db2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43db2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43db2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="43db2-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.</span><span class="sxs-lookup"><span data-stu-id="43db2-106">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="43db2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="43db2-107">Permissions</span></span>

<span data-ttu-id="43db2-p102">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43db2-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43db2-110">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="43db2-110">Resource type / Item</span></span>        | <span data-ttu-id="43db2-111">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="43db2-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="43db2-112">Kontakte</span><span class="sxs-lookup"><span data-stu-id="43db2-112">Contacts</span></span>                    | <span data-ttu-id="43db2-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="43db2-113">Contacts.Read</span></span>       |
| <span data-ttu-id="43db2-114">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="43db2-114">Conversations</span></span>               | <span data-ttu-id="43db2-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="43db2-115">Group.Read.All</span></span>      |
| <span data-ttu-id="43db2-116">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="43db2-116">Events</span></span>                      | <span data-ttu-id="43db2-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="43db2-117">Calendars.Read</span></span>      |
| <span data-ttu-id="43db2-118">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="43db2-118">Messages</span></span>                    | <span data-ttu-id="43db2-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="43db2-119">Mail.Read</span></span>           |
| <span data-ttu-id="43db2-120">Gruppen</span><span class="sxs-lookup"><span data-stu-id="43db2-120">Groups</span></span>                      | <span data-ttu-id="43db2-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="43db2-121">Group.Read.All</span></span>      |
| <span data-ttu-id="43db2-122">Benutzer</span><span class="sxs-lookup"><span data-stu-id="43db2-122">Users</span></span>                       | <span data-ttu-id="43db2-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="43db2-123">User.Read.All</span></span>       |
| <span data-ttu-id="43db2-124">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="43db2-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="43db2-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43db2-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="43db2-126">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="43db2-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="43db2-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43db2-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="43db2-128">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="43db2-128">Security alert</span></span>              | <span data-ttu-id="43db2-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43db2-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="43db2-130">***Hinweis:*** Der Endpunkt /beta kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="43db2-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="43db2-131">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43db2-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="43db2-132">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43db2-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43db2-133">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="43db2-133">Optional query parameters</span></span>

<span data-ttu-id="43db2-134">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="43db2-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43db2-135">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43db2-135">Request headers</span></span>

| <span data-ttu-id="43db2-136">Name</span><span class="sxs-lookup"><span data-stu-id="43db2-136">Name</span></span>       | <span data-ttu-id="43db2-137">Typ</span><span class="sxs-lookup"><span data-stu-id="43db2-137">Type</span></span> | <span data-ttu-id="43db2-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43db2-138">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="43db2-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="43db2-139">Authorization</span></span>  | <span data-ttu-id="43db2-140">string</span><span class="sxs-lookup"><span data-stu-id="43db2-140">string</span></span>  | <span data-ttu-id="43db2-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="43db2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43db2-143">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43db2-143">Request body</span></span>

<span data-ttu-id="43db2-144">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="43db2-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43db2-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="43db2-145">Response</span></span>

<span data-ttu-id="43db2-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43db2-146">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43db2-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43db2-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="43db2-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43db2-148">Request</span></span>

<span data-ttu-id="43db2-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43db2-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="43db2-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="43db2-150">Response</span></span>

<span data-ttu-id="43db2-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="43db2-151">Here is an example of the response.</span></span>
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
