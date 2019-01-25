---
title: Abonnement abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c7dd20810cd9fdacec697345d42690f85bc3b8b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522364"
---
# <a name="get-subscription"></a><span data-ttu-id="8ca34-103">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="8ca34-103">Get subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ca34-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Abonnements abrufen.</span><span class="sxs-lookup"><span data-stu-id="8ca34-104">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ca34-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8ca34-105">Permissions</span></span>

<span data-ttu-id="8ca34-p101">In der folgenden Tabelle ist für jede Ressource die entsprechende vorgeschlagene erforderliche Berechtigung aufgeführt. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ca34-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ca34-108">Ressourcentyp/Element</span><span class="sxs-lookup"><span data-stu-id="8ca34-108">Resource type / Item</span></span>        | <span data-ttu-id="8ca34-109">Berechtigung</span><span class="sxs-lookup"><span data-stu-id="8ca34-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="8ca34-110">Kontakte</span><span class="sxs-lookup"><span data-stu-id="8ca34-110">Contacts</span></span>                    | <span data-ttu-id="8ca34-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8ca34-111">Contacts.Read</span></span>       |
| <span data-ttu-id="8ca34-112">Unterhaltungen</span><span class="sxs-lookup"><span data-stu-id="8ca34-112">Conversations</span></span>               | <span data-ttu-id="8ca34-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ca34-113">Group.Read.All</span></span>      |
| <span data-ttu-id="8ca34-114">Ereignisse</span><span class="sxs-lookup"><span data-stu-id="8ca34-114">Events</span></span>                      | <span data-ttu-id="8ca34-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8ca34-115">Calendars.Read</span></span>      |
| <span data-ttu-id="8ca34-116">Nachrichten</span><span class="sxs-lookup"><span data-stu-id="8ca34-116">Messages</span></span>                    | <span data-ttu-id="8ca34-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8ca34-117">Mail.Read</span></span>           |
| <span data-ttu-id="8ca34-118">Gruppen</span><span class="sxs-lookup"><span data-stu-id="8ca34-118">Groups</span></span>                      | <span data-ttu-id="8ca34-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ca34-119">Group.Read.All</span></span>      |
| <span data-ttu-id="8ca34-120">Benutzer</span><span class="sxs-lookup"><span data-stu-id="8ca34-120">Users</span></span>                       | <span data-ttu-id="8ca34-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ca34-121">User.Read.All</span></span>       |
| <span data-ttu-id="8ca34-122">Laufwerk (OneDrive eines Benutzers)</span><span class="sxs-lookup"><span data-stu-id="8ca34-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="8ca34-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ca34-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="8ca34-124">Laufwerke (gemeinsame SharePoint-Inhalte und Laufwerke)</span><span class="sxs-lookup"><span data-stu-id="8ca34-124">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="8ca34-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ca34-125">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="8ca34-126">Sicherheitshinweis</span><span class="sxs-lookup"><span data-stu-id="8ca34-126">Security alert</span></span>              | <span data-ttu-id="8ca34-127">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ca34-127">SecurityEvents.ReadWrite.All</span></span> |

<span data-ttu-id="8ca34-128">***Hinweis:*** Der Endpunkt /beta kann Berechtigungen für die meisten Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="8ca34-128">***Note:*** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="8ca34-129">Unterhaltungen in einer Gruppe und OneDrive Laufwerk Stammelemente werden mit den Anwendungsberechtigungen nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ca34-129">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="8ca34-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ca34-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ca34-131">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8ca34-131">Optional query parameters</span></span>

<span data-ttu-id="8ca34-132">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8ca34-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ca34-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ca34-133">Request headers</span></span>

| <span data-ttu-id="8ca34-134">Name</span><span class="sxs-lookup"><span data-stu-id="8ca34-134">Name</span></span>       | <span data-ttu-id="8ca34-135">Typ</span><span class="sxs-lookup"><span data-stu-id="8ca34-135">Type</span></span> | <span data-ttu-id="8ca34-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ca34-136">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="8ca34-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ca34-137">Authorization</span></span>  | <span data-ttu-id="8ca34-138">string</span><span class="sxs-lookup"><span data-stu-id="8ca34-138">string</span></span>  | <span data-ttu-id="8ca34-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8ca34-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ca34-141">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ca34-141">Request body</span></span>

<span data-ttu-id="8ca34-142">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8ca34-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ca34-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ca34-143">Response</span></span>

<span data-ttu-id="8ca34-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ca34-144">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ca34-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ca34-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8ca34-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ca34-146">Request</span></span>

<span data-ttu-id="8ca34-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ca34-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="8ca34-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ca34-148">Response</span></span>

<span data-ttu-id="8ca34-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8ca34-149">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
