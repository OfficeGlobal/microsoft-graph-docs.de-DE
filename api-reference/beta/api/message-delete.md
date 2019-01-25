---
title: Nachricht löschen
description: Löschen einer Nachricht in das angegebene Postfach des Benutzers ein, oder Löschen einer Beziehung der Nachricht.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1237ba7e4aa5ab0439af9f07902705e7b4061374
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513543"
---
# <a name="delete-message"></a><span data-ttu-id="9c9df-103">Nachricht löschen</span><span class="sxs-lookup"><span data-stu-id="9c9df-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c9df-104">Löschen einer Nachricht in das angegebene Postfach des Benutzers ein, oder Löschen einer Beziehung der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="9c9df-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="9c9df-105">Beispielsweise können Sie eine bestimmte [@ Erwähnung](../resources/mention.md) des angegebenen Benutzers in der Nachricht löschen.</span><span class="sxs-lookup"><span data-stu-id="9c9df-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="9c9df-106">**Hinweis** Sie können möglicherweise nicht löschen von Elementen im Ordner "wiederherstellbare Elemente löschen" (dargestellt durch die [bekannte Ordnername](../resources/mailfolder.md) `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="9c9df-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="9c9df-107">Weitere Informationen finden Sie unter [Aufbewahrungszeit für gelöschte](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) und [Gelöschte Elemente bereinigen](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="9c9df-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c9df-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9c9df-108">Permissions</span></span>
<span data-ttu-id="9c9df-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c9df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c9df-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c9df-111">Permission type</span></span>      | <span data-ttu-id="9c9df-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c9df-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c9df-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c9df-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9c9df-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c9df-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9c9df-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c9df-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c9df-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c9df-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9c9df-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c9df-117">Application</span></span> | <span data-ttu-id="9c9df-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c9df-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c9df-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c9df-119">HTTP request</span></span>

<span data-ttu-id="9c9df-120">So löschen Sie die angegebene Meldung:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9c9df-120">To delete the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="9c9df-121">So löschen Sie eine bestimmte [erwähnen](../resources/mention.md) in einer Nachricht<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9c9df-121">To delete a specific [mention](../resources/mention.md) in a message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9c9df-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c9df-122">Request headers</span></span>
| <span data-ttu-id="9c9df-123">Name</span><span class="sxs-lookup"><span data-stu-id="9c9df-123">Name</span></span>       | <span data-ttu-id="9c9df-124">Typ</span><span class="sxs-lookup"><span data-stu-id="9c9df-124">Type</span></span> | <span data-ttu-id="9c9df-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c9df-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c9df-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c9df-126">Authorization</span></span>  | <span data-ttu-id="9c9df-127">string</span><span class="sxs-lookup"><span data-stu-id="9c9df-127">string</span></span>  | <span data-ttu-id="9c9df-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9c9df-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c9df-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c9df-130">Request body</span></span>
<span data-ttu-id="9c9df-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9c9df-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c9df-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c9df-132">Response</span></span>

<span data-ttu-id="9c9df-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c9df-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c9df-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c9df-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="9c9df-136">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="9c9df-136">Request 1</span></span>
<span data-ttu-id="9c9df-137">Im erste Beispiel löscht die angegebene Nachricht.</span><span class="sxs-lookup"><span data-stu-id="9c9df-137">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="9c9df-138">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="9c9df-138">Response 1</span></span>
<span data-ttu-id="9c9df-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9c9df-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="9c9df-140">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="9c9df-140">Request 2</span></span>
<span data-ttu-id="9c9df-141">Im nächste Beispiel löscht eine bestimmte **erwähnen** in der angegebenen Nachricht.</span><span class="sxs-lookup"><span data-stu-id="9c9df-141">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="9c9df-142">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="9c9df-142">Response 2</span></span>
<span data-ttu-id="9c9df-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9c9df-143">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
