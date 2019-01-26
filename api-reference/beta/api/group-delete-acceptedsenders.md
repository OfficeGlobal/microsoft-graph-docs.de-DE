---
title: acceptedSender entfernen
description: 'Mit dieser API können Sie Benutzer oder Gruppen aus der Liste „acceptedSenders“ entfernen. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a01c51487a2ffde821c2a4fd04c52363f7f82aa5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575534"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="b08f0-103">acceptedSender entfernen</span><span class="sxs-lookup"><span data-stu-id="b08f0-103">Remove acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b08f0-104">Mit dieser API können Sie Benutzer oder Gruppen aus der Liste „acceptedSenders“ entfernen.</span><span class="sxs-lookup"><span data-stu-id="b08f0-104">Remove a user or group from the acceptedSenders list.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b08f0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b08f0-105">Permissions</span></span>
<span data-ttu-id="b08f0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b08f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b08f0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b08f0-108">Permission type</span></span>                        | <span data-ttu-id="b08f0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b08f0-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="b08f0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b08f0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b08f0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b08f0-111">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="b08f0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b08f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b08f0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b08f0-113">Not supported.</span></span>|
| <span data-ttu-id="b08f0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b08f0-114">Application</span></span>                            | <span data-ttu-id="b08f0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b08f0-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b08f0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b08f0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=<id>
```

## <a name="request-headers"></a><span data-ttu-id="b08f0-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b08f0-117">Request headers</span></span>
| <span data-ttu-id="b08f0-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b08f0-118">Header</span></span>         | <span data-ttu-id="b08f0-119">Wert</span><span class="sxs-lookup"><span data-stu-id="b08f0-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="b08f0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b08f0-120">Authorization</span></span>  | <span data-ttu-id="b08f0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b08f0-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="b08f0-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b08f0-123">Request body</span></span>
<span data-ttu-id="b08f0-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b08f0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b08f0-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="b08f0-125">Response</span></span>
<span data-ttu-id="b08f0-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b08f0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b08f0-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b08f0-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b08f0-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b08f0-129">Request</span></span>
<span data-ttu-id="b08f0-130">Nachfolgend finden Sie ein paar Beispiele der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b08f0-130">The following are a couple of examples of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```

#### <a name="response"></a><span data-ttu-id="b08f0-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b08f0-131">Response</span></span>
<span data-ttu-id="b08f0-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b08f0-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-acceptedsenders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
