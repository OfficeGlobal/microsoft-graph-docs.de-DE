---
title: acceptedSender erstellen
description: Fügt einen neuen Benutzer oder eine neue Gruppe zur acceptedSender-Liste hinzu.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ba5d98796807be0ad1bb6eb58bb55fd8eb00fb84
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990278"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="74321-103">acceptedSender erstellen</span><span class="sxs-lookup"><span data-stu-id="74321-103">Create acceptedSender</span></span>
<span data-ttu-id="74321-104">Fügt einen neuen Benutzer oder eine neue Gruppe zur acceptedSender-Liste hinzu.</span><span class="sxs-lookup"><span data-stu-id="74321-104">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="74321-p101">Geben Sie den Benutzer oder die Gruppe in `@odata.id` im Anforderungstext an. Benutzer in der Liste der zulässigen Absender können Beiträge für Unterhaltungen der Gruppe bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für zulässige und abgelehnte Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="74321-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="74321-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="74321-108">Permissions</span></span>
<span data-ttu-id="74321-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74321-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74321-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74321-111">Permission type</span></span>      | <span data-ttu-id="74321-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74321-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74321-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74321-113">Delegated (work or school account)</span></span> | <span data-ttu-id="74321-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74321-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="74321-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74321-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74321-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74321-116">Not supported.</span></span>    |
|<span data-ttu-id="74321-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74321-117">Application</span></span> | <span data-ttu-id="74321-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74321-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74321-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74321-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="74321-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74321-120">Request headers</span></span>
| <span data-ttu-id="74321-121">Header</span><span class="sxs-lookup"><span data-stu-id="74321-121">Header</span></span>       | <span data-ttu-id="74321-122">Wert</span><span class="sxs-lookup"><span data-stu-id="74321-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74321-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74321-123">Authorization</span></span>  | <span data-ttu-id="74321-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="74321-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74321-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74321-126">Request body</span></span>
<span data-ttu-id="74321-127">Geben Sie im Anforderungstext die ID eines Benutzer- oder Gruppenobjekts an.</span><span class="sxs-lookup"><span data-stu-id="74321-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="74321-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="74321-128">Response</span></span>
<span data-ttu-id="74321-129">Diese Methode gibt den Antwortcode `204 No Content` ohne Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="74321-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="74321-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74321-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="74321-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74321-131">Request</span></span>
<span data-ttu-id="74321-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74321-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="74321-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="74321-133">Response</span></span>
<span data-ttu-id="74321-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="74321-134">The following is an example of the response.</span></span>
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
