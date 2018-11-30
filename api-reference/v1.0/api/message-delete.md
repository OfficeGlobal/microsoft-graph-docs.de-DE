---
title: Nachricht löschen
description: Löschen einer Nachricht in das angegebene Postfach des Benutzers ein, oder Löschen einer Beziehung der Nachricht.
ms.openlocfilehash: 5bfcb57f3f9c82f79147c30c982f59172e48b51f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019107"
---
# <a name="delete-message"></a><span data-ttu-id="658cc-103">Nachricht löschen</span><span class="sxs-lookup"><span data-stu-id="658cc-103">Delete message</span></span>

<span data-ttu-id="658cc-104">Löschen einer Nachricht in das angegebene Postfach des Benutzers ein, oder Löschen einer Beziehung der Nachricht.</span><span class="sxs-lookup"><span data-stu-id="658cc-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="658cc-105">**Hinweis** Sie können möglicherweise nicht löschen von Elementen im Ordner "wiederherstellbare Elemente löschen" (dargestellt durch die [bekannte Ordnername](../resources/mailfolder.md) `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="658cc-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="658cc-106">Weitere Informationen finden Sie unter [Aufbewahrungszeit für gelöschte](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) und [Gelöschte Elemente bereinigen](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="658cc-106">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="658cc-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="658cc-107">Permissions</span></span>
<span data-ttu-id="658cc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="658cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="658cc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="658cc-110">Permission type</span></span>      | <span data-ttu-id="658cc-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="658cc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="658cc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="658cc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="658cc-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="658cc-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="658cc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="658cc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="658cc-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="658cc-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="658cc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="658cc-116">Application</span></span> | <span data-ttu-id="658cc-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="658cc-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="658cc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="658cc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="658cc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="658cc-119">Request headers</span></span>
| <span data-ttu-id="658cc-120">Name</span><span class="sxs-lookup"><span data-stu-id="658cc-120">Name</span></span>       | <span data-ttu-id="658cc-121">Typ</span><span class="sxs-lookup"><span data-stu-id="658cc-121">Type</span></span> | <span data-ttu-id="658cc-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="658cc-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="658cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="658cc-123">Authorization</span></span>  | <span data-ttu-id="658cc-124">string</span><span class="sxs-lookup"><span data-stu-id="658cc-124">string</span></span>  | <span data-ttu-id="658cc-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="658cc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="658cc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="658cc-127">Request body</span></span>
<span data-ttu-id="658cc-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="658cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="658cc-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="658cc-129">Response</span></span>

<span data-ttu-id="658cc-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="658cc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="658cc-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="658cc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="658cc-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="658cc-133">Request</span></span>
<span data-ttu-id="658cc-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="658cc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="658cc-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="658cc-135">Response</span></span>
<span data-ttu-id="658cc-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="658cc-136">Here is an example of the response.</span></span> 
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