---
title: Unterhaltung löschen
description: Löschen eines conversation-Objekts.
ms.openlocfilehash: d23e57f75cb52ae0c2aab6c8525bc18d4ac0f5c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061175"
---
# <a name="delete-conversation"></a><span data-ttu-id="b598d-103">Unterhaltung löschen</span><span class="sxs-lookup"><span data-stu-id="b598d-103">Delete conversation</span></span>

> <span data-ttu-id="b598d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b598d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b598d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b598d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b598d-106">Löschen eines [conversation](../resources/conversation.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b598d-106">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b598d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b598d-107">Permissions</span></span>
<span data-ttu-id="b598d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b598d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b598d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b598d-110">Permission type</span></span>      | <span data-ttu-id="b598d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b598d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b598d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b598d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b598d-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b598d-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b598d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b598d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b598d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b598d-115">Not supported.</span></span>    |
|<span data-ttu-id="b598d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b598d-116">Application</span></span> | <span data-ttu-id="b598d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b598d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b598d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b598d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b598d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b598d-119">Request headers</span></span>
| <span data-ttu-id="b598d-120">Name</span><span class="sxs-lookup"><span data-stu-id="b598d-120">Name</span></span>       | <span data-ttu-id="b598d-121">Typ</span><span class="sxs-lookup"><span data-stu-id="b598d-121">Type</span></span> | <span data-ttu-id="b598d-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b598d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b598d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b598d-123">Authorization</span></span>  | <span data-ttu-id="b598d-124">string</span><span class="sxs-lookup"><span data-stu-id="b598d-124">string</span></span>  | <span data-ttu-id="b598d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b598d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b598d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b598d-127">Request body</span></span>
<span data-ttu-id="b598d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b598d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b598d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b598d-129">Response</span></span>
<span data-ttu-id="b598d-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b598d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b598d-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b598d-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b598d-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b598d-133">Request</span></span>
<span data-ttu-id="b598d-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b598d-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="b598d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="b598d-135">Response</span></span>
<span data-ttu-id="b598d-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b598d-136">The following is an example of the response.</span></span> 
><span data-ttu-id="b598d-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b598d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->