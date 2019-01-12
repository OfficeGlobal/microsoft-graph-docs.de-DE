---
title: Unterhaltungsthread löschen
description: Löschen eines thread-Objekts.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f4e40763a1221575fbe45e8294aad0d2e0bdf764
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935787"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="99890-103">Unterhaltungsthread löschen</span><span class="sxs-lookup"><span data-stu-id="99890-103">Delete conversation thread</span></span>

> <span data-ttu-id="99890-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="99890-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99890-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99890-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99890-106">Löschen eines [thread](../resources/conversationthread.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="99890-106">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="99890-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="99890-107">Permissions</span></span>
<span data-ttu-id="99890-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99890-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99890-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99890-110">Permission type</span></span>      | <span data-ttu-id="99890-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99890-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99890-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99890-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99890-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99890-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="99890-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99890-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99890-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99890-115">Not supported.</span></span>    |
|<span data-ttu-id="99890-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99890-116">Application</span></span> | <span data-ttu-id="99890-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99890-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99890-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99890-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="99890-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99890-119">Request headers</span></span>
| <span data-ttu-id="99890-120">Name</span><span class="sxs-lookup"><span data-stu-id="99890-120">Name</span></span>       | <span data-ttu-id="99890-121">Typ</span><span class="sxs-lookup"><span data-stu-id="99890-121">Type</span></span> | <span data-ttu-id="99890-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99890-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="99890-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99890-123">Authorization</span></span>  | <span data-ttu-id="99890-124">string</span><span class="sxs-lookup"><span data-stu-id="99890-124">string</span></span>  | <span data-ttu-id="99890-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99890-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99890-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99890-127">Request body</span></span>
<span data-ttu-id="99890-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="99890-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99890-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="99890-129">Response</span></span>
<span data-ttu-id="99890-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99890-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99890-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99890-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="99890-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99890-133">Request</span></span>
<span data-ttu-id="99890-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="99890-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="99890-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="99890-135">Response</span></span>
<span data-ttu-id="99890-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="99890-136">The following is an example of the response.</span></span> 
><span data-ttu-id="99890-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="99890-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
