---
title: conversationThread löschen
description: Mit dieser API können Sie Ressourcen des Typs „conversationThread“ löschen.
ms.openlocfilehash: 36d35c307f9e27463adc63c27745bbe33df0cd77
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058587"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="1d1aa-103">conversationThread löschen</span><span class="sxs-lookup"><span data-stu-id="1d1aa-103">Delete conversationThread</span></span>

> <span data-ttu-id="1d1aa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d1aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d1aa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d1aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d1aa-106">Mit dieser API können Sie Ressourcen des Typs „conversationThread“ löschen.</span><span class="sxs-lookup"><span data-stu-id="1d1aa-106">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d1aa-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1d1aa-107">Permissions</span></span>
<span data-ttu-id="1d1aa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d1aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d1aa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d1aa-110">Permission type</span></span>      | <span data-ttu-id="1d1aa-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d1aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d1aa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d1aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1d1aa-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d1aa-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d1aa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d1aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d1aa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d1aa-115">Not supported.</span></span>    |
|<span data-ttu-id="1d1aa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d1aa-116">Application</span></span> | <span data-ttu-id="1d1aa-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d1aa-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d1aa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d1aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1d1aa-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d1aa-119">Request headers</span></span>
| <span data-ttu-id="1d1aa-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1d1aa-120">Header</span></span>       | <span data-ttu-id="1d1aa-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1d1aa-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d1aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d1aa-122">Authorization</span></span>  | <span data-ttu-id="1d1aa-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1d1aa-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d1aa-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1d1aa-125">Request body</span></span>
<span data-ttu-id="1d1aa-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1d1aa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d1aa-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d1aa-127">Response</span></span>

<span data-ttu-id="1d1aa-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d1aa-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d1aa-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d1aa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d1aa-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d1aa-131">Request</span></span>
<span data-ttu-id="1d1aa-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d1aa-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="1d1aa-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d1aa-133">Response</span></span>
<span data-ttu-id="1d1aa-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1d1aa-134">Here is an example of the response.</span></span> 
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
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->