---
title: mailFolder löschen
description: Löscht das angegebene MailFolder oder MailSearchFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6753eaac9e02e5b6c5ff92402f13484dc458b558
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923866"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="96321-103">mailFolder löschen</span><span class="sxs-lookup"><span data-stu-id="96321-103">Delete mailFolder</span></span>

> <span data-ttu-id="96321-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="96321-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96321-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="96321-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96321-106">Löscht das angegebene [MailFolder](../resources/mailfolder.md) oder [MailSearchFolder](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="96321-106">Delete the specified [mailFolder](../resources/mailfolder.md) or [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="96321-107">Sie können einen e-Mail-Ordner anhand der Ordner-ID oder nach seiner [bekannten Ordnername](../resources/mailfolder.md)angeben, sofern vorhanden.</span><span class="sxs-lookup"><span data-stu-id="96321-107">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="96321-108">**Hinweis** Sie können möglicherweise nicht löschen von Elementen im Ordner "wiederherstellbare Elemente löschen" (dargestellt durch die bekannte Ordnername `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="96321-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="96321-109">Weitere Informationen finden Sie unter [Aufbewahrungszeit für gelöschte](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) und [Gelöschte Elemente bereinigen](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="96321-109">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="96321-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="96321-110">Permissions</span></span>
<span data-ttu-id="96321-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96321-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96321-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96321-113">Permission type</span></span>      | <span data-ttu-id="96321-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96321-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96321-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96321-115">Delegated (work or school account)</span></span> | <span data-ttu-id="96321-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96321-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="96321-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96321-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96321-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96321-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="96321-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96321-119">Application</span></span> | <span data-ttu-id="96321-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96321-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="96321-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96321-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="96321-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96321-122">Request headers</span></span>
| <span data-ttu-id="96321-123">Name</span><span class="sxs-lookup"><span data-stu-id="96321-123">Name</span></span>       | <span data-ttu-id="96321-124">Typ</span><span class="sxs-lookup"><span data-stu-id="96321-124">Type</span></span> | <span data-ttu-id="96321-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96321-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96321-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="96321-126">Authorization</span></span>  | <span data-ttu-id="96321-127">string</span><span class="sxs-lookup"><span data-stu-id="96321-127">string</span></span>  | <span data-ttu-id="96321-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="96321-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96321-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96321-130">Request body</span></span>
<span data-ttu-id="96321-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="96321-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96321-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="96321-132">Response</span></span>
<span data-ttu-id="96321-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96321-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96321-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96321-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="96321-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96321-136">Request</span></span>
<span data-ttu-id="96321-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96321-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="96321-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="96321-138">Response</span></span>
<span data-ttu-id="96321-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="96321-139">The following is an example of the response.</span></span> 
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
