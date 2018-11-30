---
title: rejectedSender erstellen
description: Fügt einen neuen Benutzer oder eine neue Gruppe zur rejectedSender-Liste hinzu.
ms.openlocfilehash: caf0e69db01b446861dce819396a1f034e5cf13c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019916"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="2e215-103">rejectedSender erstellen</span><span class="sxs-lookup"><span data-stu-id="2e215-103">Create rejectedSender</span></span>
<span data-ttu-id="2e215-104">Fügt einen neuen Benutzer oder eine neue Gruppe zur rejectedSender-Liste hinzu.</span><span class="sxs-lookup"><span data-stu-id="2e215-104">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="2e215-p101">Geben Sie den Benutzer oder die Gruppe in `@odata.id` im Anforderungstext an. Benutzer in der Liste der abgelehnten Absender können keine Beiträge in Unterhaltungen der Gruppe (im POST-Anforderungs-URL identifiziert) bereitstellen. Stellen Sie sicher, dass Sie nicht den gleichen Benutzer oder die gleiche Gruppe in den Listen für abgelehnte und zulässige Absender angeben, sonst wird ein Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2e215-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e215-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2e215-108">Permissions</span></span>
<span data-ttu-id="2e215-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e215-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e215-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e215-111">Permission type</span></span>      | <span data-ttu-id="2e215-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e215-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e215-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e215-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2e215-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e215-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2e215-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e215-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e215-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e215-116">Not supported.</span></span>    |
|<span data-ttu-id="2e215-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e215-117">Application</span></span> | <span data-ttu-id="2e215-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e215-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e215-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e215-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2e215-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e215-120">Request headers</span></span>
| <span data-ttu-id="2e215-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2e215-121">Header</span></span>       | <span data-ttu-id="2e215-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2e215-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e215-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e215-123">Authorization</span></span>  | <span data-ttu-id="2e215-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2e215-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e215-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e215-126">Request body</span></span>
<span data-ttu-id="2e215-127">Geben Sie im Anforderungstext die ID eines Benutzer- oder Gruppenobjekts an.</span><span class="sxs-lookup"><span data-stu-id="2e215-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="2e215-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e215-128">Response</span></span>
<span data-ttu-id="2e215-129">Diese Methode gibt den Antwortcode `204 No Content` ohne Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2e215-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e215-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e215-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2e215-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e215-131">Request</span></span>
<span data-ttu-id="2e215-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e215-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
#### <a name="response"></a><span data-ttu-id="2e215-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e215-133">Response</span></span>
<span data-ttu-id="2e215-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2e215-134">The following is an example of the response.</span></span>
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
