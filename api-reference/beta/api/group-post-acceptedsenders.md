---
title: acceptedSender erstellen
description: Fügt einen neuen Benutzer oder eine neue Gruppe zur acceptedSender-Liste hinzu.
ms.openlocfilehash: 7f58f1919ca592fd2ba00e091d714f020e81a6bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063640"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="6efb0-103">acceptedSender erstellen</span><span class="sxs-lookup"><span data-stu-id="6efb0-103">Create acceptedSender</span></span>

> <span data-ttu-id="6efb0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6efb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6efb0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6efb0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6efb0-106">Fügt einen neuen Benutzer oder eine neue Gruppe zur acceptedSender-Liste hinzu.</span><span class="sxs-lookup"><span data-stu-id="6efb0-106">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="6efb0-p102">Geben Sie den Benutzer oder die Gruppe in `@odata.id` im Anforderungstext an. Benutzer in der Liste der zulässigen Absender können Beiträge für Unterhaltungen der Gruppe bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für zulässige und abgelehnte Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6efb0-p102">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="6efb0-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6efb0-110">Permissions</span></span>
<span data-ttu-id="6efb0-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6efb0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6efb0-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6efb0-113">Permission type</span></span>      | <span data-ttu-id="6efb0-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6efb0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6efb0-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6efb0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6efb0-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6efb0-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6efb0-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6efb0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6efb0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6efb0-118">Not supported.</span></span>    |
|<span data-ttu-id="6efb0-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6efb0-119">Application</span></span> | <span data-ttu-id="6efb0-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6efb0-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6efb0-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6efb0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6efb0-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6efb0-122">Request headers</span></span>
| <span data-ttu-id="6efb0-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6efb0-123">Header</span></span>       | <span data-ttu-id="6efb0-124">Wert</span><span class="sxs-lookup"><span data-stu-id="6efb0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6efb0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6efb0-125">Authorization</span></span>  | <span data-ttu-id="6efb0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6efb0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6efb0-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6efb0-128">Request body</span></span>
<span data-ttu-id="6efb0-129">Geben Sie im Anforderungstext die ID eines Benutzer- oder Gruppenobjekts an.</span><span class="sxs-lookup"><span data-stu-id="6efb0-129">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="6efb0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="6efb0-130">Response</span></span>
<span data-ttu-id="6efb0-131">Diese Methode gibt den Antwortcode `204 No Content` ohne Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6efb0-131">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="6efb0-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6efb0-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6efb0-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6efb0-133">Request</span></span>
<span data-ttu-id="6efb0-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6efb0-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="6efb0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6efb0-135">Response</span></span>
<span data-ttu-id="6efb0-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6efb0-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
