---
title: Unterhaltungsthread löschen
description: Löschen eines thread-Objekts.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 24e779b528391e82f452f7bbe3153e39a3975b93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946756"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="1ec49-103">Unterhaltungsthread löschen</span><span class="sxs-lookup"><span data-stu-id="1ec49-103">Delete conversation thread</span></span>
<span data-ttu-id="1ec49-104">Löschen eines [thread](../resources/conversationthread.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1ec49-104">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ec49-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1ec49-105">Permissions</span></span>
<span data-ttu-id="1ec49-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ec49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ec49-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ec49-108">Permission type</span></span>      | <span data-ttu-id="1ec49-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ec49-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ec49-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ec49-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ec49-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ec49-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ec49-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ec49-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ec49-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ec49-113">Not supported.</span></span>    |
|<span data-ttu-id="1ec49-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ec49-114">Application</span></span> | <span data-ttu-id="1ec49-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ec49-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ec49-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ec49-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1ec49-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ec49-117">Request headers</span></span>
| <span data-ttu-id="1ec49-118">Name</span><span class="sxs-lookup"><span data-stu-id="1ec49-118">Name</span></span>       | <span data-ttu-id="1ec49-119">Typ</span><span class="sxs-lookup"><span data-stu-id="1ec49-119">Type</span></span> | <span data-ttu-id="1ec49-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ec49-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1ec49-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ec49-121">Authorization</span></span>  | <span data-ttu-id="1ec49-122">string</span><span class="sxs-lookup"><span data-stu-id="1ec49-122">string</span></span>  | <span data-ttu-id="1ec49-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1ec49-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ec49-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ec49-125">Request body</span></span>
<span data-ttu-id="1ec49-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1ec49-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ec49-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ec49-127">Response</span></span>
<span data-ttu-id="1ec49-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ec49-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ec49-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ec49-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1ec49-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ec49-131">Request</span></span>
<span data-ttu-id="1ec49-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ec49-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="1ec49-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ec49-133">Response</span></span>
<span data-ttu-id="1ec49-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1ec49-134">The following is an example of the response.</span></span> 
><span data-ttu-id="1ec49-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1ec49-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
