---
title: Unterhaltungsthread löschen
description: Löschen eines thread-Objekts.
author: dkershaw10
ms.openlocfilehash: b8dc8d2675804fabbd6c6b5dcbb7d30ad34a211c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339445"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="8bbd6-103">Unterhaltungsthread löschen</span><span class="sxs-lookup"><span data-stu-id="8bbd6-103">Delete conversation thread</span></span>
<span data-ttu-id="8bbd6-104">Löschen eines [thread](../resources/conversationthread.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8bbd6-104">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bbd6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8bbd6-105">Permissions</span></span>
<span data-ttu-id="8bbd6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bbd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bbd6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8bbd6-108">Permission type</span></span>      | <span data-ttu-id="8bbd6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8bbd6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bbd6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8bbd6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8bbd6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bbd6-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8bbd6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8bbd6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bbd6-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8bbd6-113">Not supported.</span></span>    |
|<span data-ttu-id="8bbd6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8bbd6-114">Application</span></span> | <span data-ttu-id="8bbd6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8bbd6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bbd6-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8bbd6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8bbd6-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8bbd6-117">Request headers</span></span>
| <span data-ttu-id="8bbd6-118">Name</span><span class="sxs-lookup"><span data-stu-id="8bbd6-118">Name</span></span>       | <span data-ttu-id="8bbd6-119">Typ</span><span class="sxs-lookup"><span data-stu-id="8bbd6-119">Type</span></span> | <span data-ttu-id="8bbd6-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8bbd6-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8bbd6-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8bbd6-121">Authorization</span></span>  | <span data-ttu-id="8bbd6-122">string</span><span class="sxs-lookup"><span data-stu-id="8bbd6-122">string</span></span>  | <span data-ttu-id="8bbd6-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8bbd6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bbd6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8bbd6-125">Request body</span></span>
<span data-ttu-id="8bbd6-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8bbd6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bbd6-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="8bbd6-127">Response</span></span>
<span data-ttu-id="8bbd6-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8bbd6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bbd6-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8bbd6-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8bbd6-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8bbd6-131">Request</span></span>
<span data-ttu-id="8bbd6-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8bbd6-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="8bbd6-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8bbd6-133">Response</span></span>
<span data-ttu-id="8bbd6-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8bbd6-134">The following is an example of the response.</span></span> 
><span data-ttu-id="8bbd6-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8bbd6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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