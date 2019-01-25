---
title: Unterhaltung löschen
description: Löschen eines conversation-Objekts.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d807f3bcd2a933486cd3742ed3828c1c009a6f03
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529663"
---
# <a name="delete-conversation"></a><span data-ttu-id="f7181-103">Unterhaltung löschen</span><span class="sxs-lookup"><span data-stu-id="f7181-103">Delete conversation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7181-104">Löschen eines [conversation](../resources/conversation.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f7181-104">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7181-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f7181-105">Permissions</span></span>
<span data-ttu-id="f7181-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7181-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7181-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7181-108">Permission type</span></span>      | <span data-ttu-id="f7181-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7181-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7181-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7181-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7181-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7181-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7181-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7181-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7181-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7181-113">Not supported.</span></span>    |
|<span data-ttu-id="f7181-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7181-114">Application</span></span> | <span data-ttu-id="f7181-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f7181-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7181-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7181-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f7181-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7181-117">Request headers</span></span>
| <span data-ttu-id="f7181-118">Name</span><span class="sxs-lookup"><span data-stu-id="f7181-118">Name</span></span>       | <span data-ttu-id="f7181-119">Typ</span><span class="sxs-lookup"><span data-stu-id="f7181-119">Type</span></span> | <span data-ttu-id="f7181-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7181-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7181-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7181-121">Authorization</span></span>  | <span data-ttu-id="f7181-122">string</span><span class="sxs-lookup"><span data-stu-id="f7181-122">string</span></span>  | <span data-ttu-id="f7181-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f7181-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7181-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7181-125">Request body</span></span>
<span data-ttu-id="f7181-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f7181-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7181-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7181-127">Response</span></span>
<span data-ttu-id="f7181-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7181-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7181-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7181-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f7181-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7181-131">Request</span></span>
<span data-ttu-id="f7181-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f7181-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="f7181-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7181-133">Response</span></span>
<span data-ttu-id="f7181-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f7181-134">The following is an example of the response.</span></span> 
><span data-ttu-id="f7181-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f7181-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-conversation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
