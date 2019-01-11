---
title: Abonnement abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.
localization_priority: Normal
ms.openlocfilehash: 0feb4ffd49099eabb92e5519b25233100f2acbe5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846837"
---
# <a name="get-subscription"></a><span data-ttu-id="8749c-103">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="8749c-103">Get subscription</span></span>

> <span data-ttu-id="8749c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8749c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8749c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8749c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8749c-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.</span><span class="sxs-lookup"><span data-stu-id="8749c-106">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="8749c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8749c-107">Permissions</span></span>

<span data-ttu-id="8749c-p102">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8749c-p102">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8749c-110">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="8749c-110">Resource type / Item</span></span>        | <span data-ttu-id="8749c-111">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="8749c-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="8749c-112">Kontakte</span><span class="sxs-lookup"><span data-stu-id="8749c-112">Contacts</span></span>                    | <span data-ttu-id="8749c-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8749c-113">Contacts.Read</span></span>       |
| <span data-ttu-id="8749c-114">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="8749c-114">Conversations</span></span>               | <span data-ttu-id="8749c-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8749c-115">Group.Read.All</span></span>      |
| <span data-ttu-id="8749c-116">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="8749c-116">Events</span></span>                      | <span data-ttu-id="8749c-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8749c-117">Calendars.Read</span></span>      |
| <span data-ttu-id="8749c-118">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="8749c-118">Messages</span></span>                    | <span data-ttu-id="8749c-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8749c-119">Mail.Read</span></span>           |
| <span data-ttu-id="8749c-120">Gruppen</span><span class="sxs-lookup"><span data-stu-id="8749c-120">Groups</span></span>                      | <span data-ttu-id="8749c-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8749c-121">Group.Read.All</span></span>      |
| <span data-ttu-id="8749c-122">Benutzer</span><span class="sxs-lookup"><span data-stu-id="8749c-122">Users</span></span>                       | <span data-ttu-id="8749c-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8749c-123">User.Read.All</span></span>       |
| <span data-ttu-id="8749c-124">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="8749c-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="8749c-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8749c-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="8749c-126">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="8749c-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="8749c-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8749c-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="8749c-128">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="8749c-128">Security alert</span></span>              | <span data-ttu-id="8749c-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8749c-129">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="8749c-130">***Hinweis:*** Der Endpunkt /beta kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="8749c-130">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="8749c-131">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8749c-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="8749c-132">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8749c-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8749c-133">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8749c-133">Optional query parameters</span></span>

<span data-ttu-id="8749c-134">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8749c-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8749c-135">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8749c-135">Request headers</span></span>

| <span data-ttu-id="8749c-136">Name</span><span class="sxs-lookup"><span data-stu-id="8749c-136">Name</span></span>       | <span data-ttu-id="8749c-137">Typ</span><span class="sxs-lookup"><span data-stu-id="8749c-137">Type</span></span> | <span data-ttu-id="8749c-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8749c-138">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="8749c-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="8749c-139">Authorization</span></span>  | <span data-ttu-id="8749c-140">string</span><span class="sxs-lookup"><span data-stu-id="8749c-140">string</span></span>  | <span data-ttu-id="8749c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8749c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8749c-143">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8749c-143">Request body</span></span>

<span data-ttu-id="8749c-144">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8749c-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8749c-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="8749c-145">Response</span></span>

<span data-ttu-id="8749c-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8749c-146">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8749c-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8749c-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8749c-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8749c-148">Request</span></span>

<span data-ttu-id="8749c-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8749c-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="8749c-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="8749c-150">Response</span></span>

<span data-ttu-id="8749c-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8749c-151">Here is an example of the response.</span></span>
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
