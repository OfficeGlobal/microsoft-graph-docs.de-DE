---
title: mailFolder löschen
description: Löschen der angegebenen MailFolder.
ms.openlocfilehash: e01f631141147373d1c2010d4313ad833c057df2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019897"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="ebdbe-103">mailFolder löschen</span><span class="sxs-lookup"><span data-stu-id="ebdbe-103">Delete mailFolder</span></span>

<span data-ttu-id="ebdbe-104">Löschen der angegebenen [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ebdbe-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span>

<span data-ttu-id="ebdbe-105">Sie können einen e-Mail-Ordner anhand der Ordner-ID oder nach seiner [bekannten Ordnername](../resources/mailfolder.md)angeben, sofern vorhanden.</span><span class="sxs-lookup"><span data-stu-id="ebdbe-105">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="ebdbe-106">**Hinweis** Sie können möglicherweise nicht löschen von Elementen im Ordner "wiederherstellbare Elemente löschen" (dargestellt durch die bekannte Ordnername `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="ebdbe-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="ebdbe-107">Weitere Informationen finden Sie unter [Aufbewahrungszeit für gelöschte](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) und [Gelöschte Elemente bereinigen](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="ebdbe-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebdbe-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ebdbe-108">Permissions</span></span>
<span data-ttu-id="ebdbe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebdbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebdbe-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ebdbe-111">Permission type</span></span>      | <span data-ttu-id="ebdbe-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ebdbe-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebdbe-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ebdbe-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ebdbe-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebdbe-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ebdbe-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ebdbe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebdbe-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebdbe-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ebdbe-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ebdbe-117">Application</span></span> | <span data-ttu-id="ebdbe-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebdbe-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebdbe-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebdbe-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ebdbe-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ebdbe-120">Request headers</span></span>
| <span data-ttu-id="ebdbe-121">Name</span><span class="sxs-lookup"><span data-stu-id="ebdbe-121">Name</span></span>       | <span data-ttu-id="ebdbe-122">Typ</span><span class="sxs-lookup"><span data-stu-id="ebdbe-122">Type</span></span> | <span data-ttu-id="ebdbe-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebdbe-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ebdbe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebdbe-124">Authorization</span></span>  | <span data-ttu-id="ebdbe-125">string</span><span class="sxs-lookup"><span data-stu-id="ebdbe-125">string</span></span>  | <span data-ttu-id="ebdbe-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ebdbe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebdbe-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ebdbe-128">Request body</span></span>
<span data-ttu-id="ebdbe-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ebdbe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebdbe-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebdbe-130">Response</span></span>

<span data-ttu-id="ebdbe-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebdbe-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebdbe-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ebdbe-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebdbe-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebdbe-134">Request</span></span>
<span data-ttu-id="ebdbe-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ebdbe-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="ebdbe-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebdbe-136">Response</span></span>
<span data-ttu-id="ebdbe-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ebdbe-137">Here is an example of the response.</span></span> 
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->