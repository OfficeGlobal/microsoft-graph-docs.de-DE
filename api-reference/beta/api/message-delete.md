---
title: Nachricht löschen
description: Löschen einer Nachricht in das angegebene Postfach des Benutzers ein, oder Löschen einer Beziehung der Nachricht.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8ef6636e98d516bab1dea29c37dcc23caa7a01ed
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942444"
---
# <a name="delete-message"></a><span data-ttu-id="1d559-103">Nachricht löschen</span><span class="sxs-lookup"><span data-stu-id="1d559-103">Delete message</span></span>

> <span data-ttu-id="1d559-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d559-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d559-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d559-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d559-106">Löschen einer Nachricht in das angegebene Postfach des Benutzers ein, oder Löschen einer Beziehung der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="1d559-106">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="1d559-107">Beispielsweise können Sie eine bestimmte [@ Erwähnung](../resources/mention.md) des angegebenen Benutzers in der Nachricht löschen.</span><span class="sxs-lookup"><span data-stu-id="1d559-107">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="1d559-108">**Hinweis** Sie können möglicherweise nicht löschen von Elementen im Ordner "wiederherstellbare Elemente löschen" (dargestellt durch die [bekannte Ordnername](../resources/mailfolder.md) `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="1d559-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="1d559-109">Weitere Informationen finden Sie unter [Aufbewahrungszeit für gelöschte](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) und [Gelöschte Elemente bereinigen](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="1d559-109">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d559-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1d559-110">Permissions</span></span>
<span data-ttu-id="1d559-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d559-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d559-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d559-113">Permission type</span></span>      | <span data-ttu-id="1d559-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d559-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d559-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d559-115">Delegated (work or school account)</span></span> | <span data-ttu-id="1d559-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d559-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1d559-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d559-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d559-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d559-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1d559-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d559-119">Application</span></span> | <span data-ttu-id="1d559-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d559-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d559-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d559-121">HTTP request</span></span>

<span data-ttu-id="1d559-122">So löschen Sie die angegebene Meldung:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="1d559-122">To delete the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="1d559-123">So löschen Sie eine bestimmte [erwähnen](../resources/mention.md) in einer Nachricht<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="1d559-123">To delete a specific [mention](../resources/mention.md) in a message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1d559-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d559-124">Request headers</span></span>
| <span data-ttu-id="1d559-125">Name</span><span class="sxs-lookup"><span data-stu-id="1d559-125">Name</span></span>       | <span data-ttu-id="1d559-126">Typ</span><span class="sxs-lookup"><span data-stu-id="1d559-126">Type</span></span> | <span data-ttu-id="1d559-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d559-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d559-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d559-128">Authorization</span></span>  | <span data-ttu-id="1d559-129">string</span><span class="sxs-lookup"><span data-stu-id="1d559-129">string</span></span>  | <span data-ttu-id="1d559-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1d559-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d559-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1d559-132">Request body</span></span>
<span data-ttu-id="1d559-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1d559-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d559-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d559-134">Response</span></span>

<span data-ttu-id="1d559-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d559-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d559-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d559-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="1d559-138">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="1d559-138">Request 1</span></span>
<span data-ttu-id="1d559-139">Im erste Beispiel löscht die angegebene Nachricht.</span><span class="sxs-lookup"><span data-stu-id="1d559-139">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="1d559-140">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="1d559-140">Response 1</span></span>
<span data-ttu-id="1d559-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1d559-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="1d559-142">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="1d559-142">Request 2</span></span>
<span data-ttu-id="1d559-143">Im nächste Beispiel löscht eine bestimmte **erwähnen** in der angegebenen Nachricht.</span><span class="sxs-lookup"><span data-stu-id="1d559-143">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="1d559-144">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="1d559-144">Response 2</span></span>
<span data-ttu-id="1d559-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1d559-145">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
