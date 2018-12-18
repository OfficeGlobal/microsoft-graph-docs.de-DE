---
title: acceptedSender entfernen
description: 'Mit dieser API können Sie Benutzer oder Gruppen aus der Liste „acceptedSenders“ entfernen. '
author: dkershaw10
ms.openlocfilehash: 7f175be4e7f3acc470170d863a43c36db42299b0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329771"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="e9c3e-103">acceptedSender entfernen</span><span class="sxs-lookup"><span data-stu-id="e9c3e-103">Remove acceptedSender</span></span>
<span data-ttu-id="e9c3e-104">Mit dieser API können Sie Benutzer oder Gruppen aus der Liste „acceptedSenders“ entfernen.</span><span class="sxs-lookup"><span data-stu-id="e9c3e-104">Remove a user or group from the acceptedSenders list.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e9c3e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e9c3e-105">Permissions</span></span>
<span data-ttu-id="e9c3e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9c3e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e9c3e-108">Permission type</span></span>                        | <span data-ttu-id="e9c3e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e9c3e-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="e9c3e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e9c3e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9c3e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9c3e-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="e9c3e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e9c3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9c3e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e9c3e-113">Not supported.</span></span> |
| <span data-ttu-id="e9c3e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e9c3e-114">Application</span></span>                            | <span data-ttu-id="e9c3e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e9c3e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9c3e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9c3e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="e9c3e-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e9c3e-117">Request headers</span></span>
| <span data-ttu-id="e9c3e-118">Header</span><span class="sxs-lookup"><span data-stu-id="e9c3e-118">Header</span></span>         | <span data-ttu-id="e9c3e-119">Wert</span><span class="sxs-lookup"><span data-stu-id="e9c3e-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="e9c3e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9c3e-120">Authorization</span></span>  | <span data-ttu-id="e9c3e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e9c3e-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="e9c3e-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e9c3e-123">Request body</span></span>
<span data-ttu-id="e9c3e-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e9c3e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9c3e-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9c3e-125">Response</span></span>
<span data-ttu-id="e9c3e-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e9c3e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9c3e-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e9c3e-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e9c3e-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9c3e-129">Request</span></span>
<span data-ttu-id="e9c3e-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e9c3e-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="e9c3e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9c3e-131">Response</span></span>
<span data-ttu-id="e9c3e-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e9c3e-132">The following is an example of the response.</span></span> 

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
